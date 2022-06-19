## Trust

Clinicians need to have absolute trust in the veracity of information in the clinical record, so GitEHR has been designed to ensure that, while it remains a distributed and decentralised system, the information contained within is completely trustworthy.

This is achieved using simple, existing, reliable and trusted technology which is widely used to establish trust in other parts of tech:

* crpytographic signatures
* cryptographic hashes

In fact, using these technologies to sign and audit-trail commits to the clinical record represents a significant advance on the current 'state of the art'.

### Existing audit-trailing is broken

In a typical Electronic Health Record (EHR) program in use today in healthcare organisations across the world, the clinical entries are saved into a database, and often (but not always!) there is an audit-trail built into the system, which ensures that if, for example, a nefarious user changed an entry *after* an adverse incident in order to avoid accountability, the tampering would be evident to the admins of such a system.

But what is **never** seemingly challenged here is that this puts the locus of trust **entirely** with the admins of the EHR, the organisation's leadership itself, and also in the design of the EHR. If you think you can put your trust unequivocally within databases, admins, and more importantly the leaders of large organisations, then you are wrong.

Here is a cautionary tale of why, as a clinician, you can't trust your life and career to these things: [The UK Post Office Scandal](https://en.wikipedia.org/wiki/British_Post_Office_scandal). In a miscarriage of justice of monumental proportions in the UK, a series of errors occurred in the system used to manage the Post Office's banking service. This resulted in large discrepancies including huge shortfalls of cash in the cash drawers at the end of the day.

Every single one of these discrepancies was the *fault of the system and its design*. However its admins believed the system, not the users. The IT company which built the system believed the system, not the users.

The Post Office's senior leadership backed the system for which they'd paid millions, not their own staff.

A number of people were jailed, some committed suicide, many thousands of lives were ruined. An audit-trail system was built into this system but it didn't work.

It's all too easy to imagine similar discrepancies occurring in clinical records. A really simple example is if the system failed to show a severe allergy alert to a clinician, and that clinician administers a drug which kills the patient. The system at fault but nobody will believe the clinician. It is far easier to scapegoat a clinician than to blame the multi-million pound EHR. The system admins will want to believe the EHR. The organisational leadership will want to believe the EHR.

It's also possible that someone with admin access might be induced to change something in the audit-trail, which in current EHRs would be essentially undetectable.

### Why GitEHR is different


Entries in a GitEHR are each cryptographically signed, meaning that the content of the entry is followed by a cryptographic signature of the content, which can be mathematically proven to have been created using the private key of the clinician. Assuming the private keys are kept properly secure, **there's nobody else on the planet who could have made that entry.**

If any change is made to the content of the clinical entry, the cryptographic signature would be invalid, immediately exposing the amendment.

Entries in a GitEHR are sequential, with each commit having a direct parent commit. In this way, commits cannot be reordered without changing the content, again such amendment would be immediately obvious.

There is frequently a valid need to make a factual change to a clinical entry, and GitEHR supports this, by simply making the update a transparent, visible process in the commit tree. The record shows the updated version, which is often clinically safer, but the previous value can be viewed and it is entirely clear who made the change and why.

GitEHR is completely open source, meaning that 'with enough eyes looking at a problem, all bugs are shallow' and we can expect that these most fundamental of GitEHR trust features will be extremely safe and reliable.