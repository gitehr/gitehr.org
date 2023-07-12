# Longevity

Health records need to last a long time. In some cases they will exist before a person is born, and last until well after their death.

However healthcare software is a different matter. Like all software there is a lifecycle to its existence. Companies start, some fail, some grow, some get acquired by bigger companies, some get dissolved, and others go bust. I think it's fair to say that software tends not to live as long as humans.

In the current closed-source EHR world, we as users and managers of patient data don't have access to the source code of these software platforms. And sadly, because of the inseparably tight coupling of the patient record data structure to the database used inside the software platform, when software dies, it's very hard to salvage the patient data in any usable form.

We need to ensure that patient records stand alone, separately from the database structure of any single proprietary software supplier.

GitEHR separates the clinical record entirely from the software used to view it.

The use of very old and simple technologies (flat files, directories, disks) helps to reduce the dependence that GitEHR has on the **new and shiny**, and makes it much more likely that as obsolete viewing and editing software reaches the end of its life, new software can be brought in to replace it pretty much seamlessly, and without affecting clinical care.