# Patient-centricity

For as long as I can remember, informaticians and health technologists have been proposing the idea of 'Patient Centric Health Records'. But they have been unable to deliver a patient-centric record because the EHR uses a database and is thereby already inherently **organisation-centric**.

!!! success 
    Understanding the above is the single most important step to seeing why we cannot make further progress in EHRs without changing the paradigm.
    
## One patient, one record

A GitEHR clinical record is only ever the record of **one** patient.

This ensures clean separation for the data in any other patient records and organisational data.

Organisations giving care keep a local record of the patient's care.

## Separation from Organisational information

A GitEHR clinical reecord is completely separated from the records of other patients and any organisation-level information. This separation allows multiple organisations to be able to contribute to the GitEHR, in the same way that multiple contributors can work on the same Git repository.

This separation also means that if, within your organisation, you need to perform database operations over multiple patients, then you can do this.

A healthcare organisation might care for thousands or even millions of patients, so it is accepted that a database at organisation level might be useful. But this database must never be the canonical patient record.

