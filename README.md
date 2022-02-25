[![Build Status](https://travis-ci.org/OpenSRP/opensrp-client-anc.svg?branch=master)](https://travis-ci.org/OpenSRP/opensrp-client-anc) [![Coverage Status](https://coveralls.io/repos/github/OpenSRP/opensrp-client-anc/badge.svg?branch=master)](https://coveralls.io/github/OpenSRP/opensrp-client-anc?branch=master)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/4a58cd4e1748432780ac66a9fbee0394)](https://www.codacy.com/app/opensrp/opensrp-client-anc?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=opensrp/opensrp-client-anc&amp;utm_campaign=Badge_Grade)
[![CodeFactor](https://www.codefactor.io/repository/github/opensrp/opensrp-client-anc/badge)](https://www.codefactor.io/repository/github/opensrp/opensrp-client-anc)

# opensrp-client-anc
The OpenSRP Antenatal Care (ANC) Reference mobile application digitizes the World Health Organization's (WHO's) latest [ANC guidelines](https://www.who.int/reproductivehealth/publications/maternal_perinatal_health/anc-positive-pregnancy-experience/en/) for routine care during pregnancy to ensure a positive outcome and experience for the pregnant woman. 

The application is geared towards ANC healthcare providers at primary healthcare facilities. Healthcare workers use the application to register pregnant women and track their routine care during pregnancy, in accordance with the latest WHO guidelines and recommendations around nutrition and dietary supplementation, maternal and fetal assessment, laboratory testing, and counseling and service provision. 

Countries are meant to use the reference application as a starting point and adapt the module to their context-specific ANC guidelines.

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Prerequisites
[Tools and Frameworks Setup](https://smartregister.atlassian.net/wiki/spaces/Documentation/pages/6619207/Tools+and+Frameworks+Setup)

## Development setup

### Steps to set up
[OpenSRP android client app build](https://smartregister.atlassian.net/wiki/spaces/Documentation/pages/6619236/OpenSRP+App+Build)

### Running the tests

[Android client unit tests](https://smartregister.atlassian.net/wiki/spaces/Documentation/pages/65570428/OpenSRP+Client)

## Deployment
[Production releases](https://smartregister.atlassian.net/wiki/spaces/Documentation/pages/1141866503/How+to+create+a+release+APK)

## Features

### Library-specific
The features below are specific to this ANC library. Dependencies to other libraries are noted in the third column.

|Function                            |Feature                                                                                                                                                                                        |Dependencies                                                       |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------|
|Server Settings                     |Set the site characteristics for your facility on first login                                                                                                                                  |                                                                   |
|Server Settings                     |View and edit the site characteristics for your facility                                                                                                                                       |                                                                   |
|Server Settings                     |Site characteristics sync between all devices of team members                                                                                                                                  |opensrp-client-core                                                |
|Server Settings                     |Set and update the population characteristics                                                                                                                                                  |opensrp-web, opensrp-server-web, opensrp-client-core               |
|Server Settings                     |View the population characteristics on the device                                                                                                                                              |opensrp-client-core                                                |
|Server Settings                     |Sync configured forms for the ANC contact visits from OpenSRP server (in progress)                                                                                                             |opensrp-server-web, opensrp-client-core, opensrp-client-native-form|
|Client Identification & Registration|Register a pregnant woman                                                                                                                                                                      |opensrp-client-core, opensrp-client-native-form                    |
|Client Identification & Registration|Edit the registration info                                                                                                                                                                     |opensrp-client-core, opensrp-client-native-form                    |
|Client Management                   |Record the woman's pregnancy outcome                                                                                                                                                           |opensrp-client-core, opensrp-client-native-form                    |
|Client Management                   |Close the ANC record after pregnancy outcome                                                                                                                                                   |opensrp-client-core                                                |
|Client Management                   |View an overview of the woman's pregnancy                                                                                                                                                      |opensrp-client-native-form (rules engine)                          |
|Client Management                   |View a summary of all previous contacts                                                                                                                                                        |opensrp-client-native-form (rules engine)                          |
|Client Management                   |View a summary of all test results                                                                                                                                                             |opensrp-client-native-form (rules engine)                          |
|Client Management                   |View pending tasks from the woman's most recent contact visit                                                                                                                                  |opensrp-client-native-form                                         |
|Client Management                   |Complete pending tasks outside the contact visit                                                                                                                                               |opensrp-client-native-form                                         |
|Client Management                   |Complete a "Quick Check" at the start of the ANC contact visit (reason for visit, complaints, danger signs)                                                                                    |opensrp-client-native-form                                         |
|Client Management                   |Refer and close a contact if a danger sign is selected                                                                                                                                         |opensrp-client-native-form                                         |
|Client Management                   |Collect demographic information at first contact                                                                                                                                               |opensrp-client-native-form                                         |
|Client Management                   |Collect Obstetric History information at first contact                                                                                                                                         |opensrp-client-native-form                                         |
|Client Management                   |Collect medical history information at first contact                                                                                                                                           |opensrp-client-native-form                                         |
|Client Management                   |Collect immunization status at first contact                                                                                                                                                   |opensrp-client-native-form                                         |
|Client Management                   |Collect Medication history at first contact                                                                                                                                                    |opensrp-client-native-form                                         |
|Client Management                   |Collect information on behaviors that affect the pregnancy at first contact                                                                                                                    |opensrp-client-native-form                                         |
|Client Management                   |Collect information on the woman's partner's HIV status at first contact                                                                                                                       |opensrp-client-native-form                                         |
|Client Management                   |Check for physiological symptoms at each contact visit                                                                                                                                         |opensrp-client-native-form                                         |
|Client Management                   |Check for persistent physiological symptoms at follow-up visits                                                                                                                                |opensrp-client-native-form                                         |
|Client Management                   |Check for compliance and side-effects of prescribed medications                                                                                                                                |opensrp-client-native-form                                         |
|Client Management                   |Conduct a full physical exam of the woman at each contact visit, including height, weight, blood pressure, temperature, pulse rate, pallor.                                                    |opensrp-client-native-form                                         |
|Client Management                   |Conduct additional, optional exams on the woman, including respiratory exam, cardiac exam, breast exam, abdominal exam, pelvic exam, cervical exam, and oedema check                           |opensrp-client-native-form                                         |
|Client Management                   |Conduct a full fetal assessment at each contact visit, including SFH, fetal movement, fetal heartbeat, and number of fetuses                                                                   |opensrp-client-native-form                                         |
|Client Management                   |View all tests that are due for the pregnant woman at that contact visit, including: Ultrasound, Blood type, HIV, Partner HIV, Hep B, Hep C, Syphilis, Urine, Blood glucose, Hemoglobin, and TB|opensrp-client-native-form                                         |
|Client Management                   |Record the type of test that was conducted                                                                                                                                                     |opensrp-client-native-form                                         |
|Client Management                   |Record results for all tests that were conducted at the visit                                                                                                                                  |opensrp-client-native-form                                         |
|Client Management                   |Record tests that were not able to be completed during the visit and reason why                                                                                                                |opensrp-client-native-form                                         |
|Client Management                   |Record tests that were ordered at the contact visit                                                                                                                                            |opensrp-client-native-form                                         |
|Client Management                   |Manual input of other test results not part of the list of tests included in the module                                                                                                        |opensrp-client-native-form                                         |
|Client Management                   |Record that the woman was referred to the hospital                                                                                                                                             |opensrp-client-native-form                                         |
|Client Management                   |Record diet counseling that was conducted                                                                                                                                                      |opensrp-client-native-form                                         |
|Client Management                   |Record treatments provided for diagnoses                                                                                                                                                       |opensrp-client-native-form                                         |
|Client Management                   |Record treatments provided to manage risks                                                                                                                                                     |opensrp-client-native-form                                         |
|Client Management                   |Record generic counseling topics that were conducted                                                                                                                                           |opensrp-client-native-form                                         |
|Client Management                   |Record whether an Intimate Partner Violence (IPV) clinical enquiry was conducted                                                                                                               |opensrp-client-native-form                                         |
|Client Management                   |Record nutrition supplementations that were prescribed                                                                                                                                         |opensrp-client-native-form                                         |
|Client Management                   |Record what deworming and malaria prophylaxis measures were provided                                                                                                                           |opensrp-client-native-form                                         |
|Client Management                   |Record what immunizations were provided                                                                                                                                                        |opensrp-client-native-form                                         |
|Client Management                   |View a summary of the entire contact visit before submitting                                                                                                                                   |opensrp-client-native-form                                         |
|Client Management                   |Finalize and submit an ANC contact visit                                                                                                                                                            |opensrp-client-core                                                |
|Service Delivery Support            |View ANC clinical reference materials in a Library                                                                                                                                                 |                                                                   |
|Service Delivery Support            |View the total number of pregnant women registered                                                                                                                                             |opensrp-client-core                                                |
|Service Delivery Support            |View a list of all registered pregnant women by most recently updated                                                                                                                          |opensrp-client-core                                                |
|Service Delivery Support            |Calculate the contact visit schedule for each pregnant woman                                                                                                                                   |opensrp-client-native-form (rules engine)                          |
|Service Delivery Support            |Calculate and display "attention flags" for each woman based on risk and health condition                                                                                                      |opensrp-client-native-form (rules engine)                          |
|Service Delivery Support            |Automatically calculate EDD and GA and update woman's GA as her pregnancy progresses                                                                                                           |opensrp-client-native-form (rules engine)                          |
|Service Delivery Support            |View the next contact visit date for the pregnant woman                                                                                                                                        |opensrp-client-native-form (rules engine)                          |
|Service Delivery Support            |Save a contact visit in progress                                                                                                                                                               |                                                                   |
|Service Delivery Support            |View contact visits in progress                                                                                                                                                                |opensrp-client-native-form (rules engine)                          |
|Service Delivery Support            |View women who are due to deliver                                                                                                                                                              |opensrp-client-core, opensrp-client-native-form                    |
|Service Delivery Support            |View contact visits that are overdue                                                                                                                                                           |opensrp-client-core, opensrp-client-native-form                    |
|Service Delivery Support            |Call the pregnant woman                                                                                                                                                                        |                                                                   |
|Service Delivery Support            |Discard changes to a contact visit before exiting                                                                                                                                              |                                                                   |
|Service Delivery Support            |Ability to show progress in the contact visit (how many required fields remain)                                                                                                                |opensrp-client-native-form                                         |
|Service Delivery Support            |Calculate EDD and GA from LMP, ultrasound and/or SFH at first contact                                                                                                                          |opensrp-client-native-form (rules engine)                          |
|Service Delivery Support            |Allow the health worker to select which method of EDD/GA calculate to use at first contact                                                                                                     |opensrp-client-native-form                                         |
|Service Delivery Support            |Automatically calculate risk based on inputs                                                                                                                                                   |opensrp-client-native-form (rules engine)                          |
|Service Delivery Support            |Diagnosis and Treatment decision support algorithms for all major pregnancy conditions                                                                                                         |opensrp-client-native-form (rules engine)                          |
|Service Delivery Support            |Decision support algorithms for all WHO ANC guidelines                                                                                                                                         |opensrp-client-native-form (rules engine)                          |

### Not library-specific
The features below are not specific to this library (i.e. the feature exists in a separate core library, but the feature is implemented as part of this library). The core library where the feature exists is noted in the third column.

|Function                            |Feature                                                                                                                                                                                        |Core Library                                                       |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------|
|Location, User and Team Management  |Use locations, teams and users created in OpenMRS                                                                                                                                              |OpenMRS, opensrp-server-web, opensrp-client-core                   |
|Location, User and Team Management  |Log in with username/password                                                                                                                                                                  |opensrp-client-core                                                |
|Location, User and Team Management  |Log out of the application                                                                                                                                                                     |opensrp-client-core                                                |
|User Settings                       |Display user's name and location                                                                                                                                                               |opensrp-client-core                                                |
|User Settings                       |Change app language                                                                                                                                                                            |opensrp-client-native-form                                         |
|User Settings                       |Display the app version and build date                                                                                                                                                         |opensrp-client-core                                                |
|User Settings                       |Display the last successful data sync date and time                                                                                                                                            |opensrp-client-core                                                |
|User Settings                       |Multi-language support for forms                                                                                                                                                               |opensrp-client-native-form                                         |
|Data Syncing                        |Manual sync in between automatic sync attempts                                                                                                                                                 |opensrp-client-core                                                |
|Client Identification & Registration|Take a picture of the pregnant woman                                                                                                                                                           |opensrp-client-native-form                                         |
|Client Identification & Registration|Auto-assign a 7-digit unique ID                                                                                                                                                                |opensrp-client-native-form                                         |
|Client Identification & Registration|Scan a QR code to override the system client ID                                                                                                                                                |opensrp-client-native-form                                         |
|Client Identification & Registration|Compute age from DOB                                                                                                                                                                           |opensrp-client-native-form                                         |
|Client Identification & Registration|Enroll the client in SMS messages                                                                                                                                                              |opensrp-client-native-form, opensrp-server-web, RapidPro           |
|Search for a Record                 |Search by name or ID                                                                                                                                                                           |opensrp-client-core                                                |
|Search for a Record                 |Advanced search by name, ID, EDD, DOB, phone number, and alternate contact name                                                                                                                |opensrp-client-core                                                |
|Search for a Record                 |Search within or outside the facility                                                                                                                                                          |opensrp-client-core                                                |
|Search for a Record                 |Scan QR code to retrieve a record                                                                                                                                                              |opensrp-client-core                                                |

## Versioning
We use SemVer for versioning. For the versions available, see the tags on this repository.
For more details check out <https://semver.org/>

## Authors/Team 
-   The OpenSRP team
-   See the list of contributors who participated in this project from the [Contributors](../../graphs/contributors) link

## Contributing
[Contribution guidelines](https://smartregister.atlassian.net/wiki/spaces/Documentation/pages/6619193/OpenSRP+Developer+s+Guide)

## Documentation
Wiki [OpenSRP Documentation](https://smartregister.atlassian.net/wiki/spaces/Documentation)

## Support
Email: <mailto:support@ona.io>
Slack workspace: <opensrp.slack.com>

## License
This project is licensed under the Apache 2.0 License - see the LICENSE.md file for details
