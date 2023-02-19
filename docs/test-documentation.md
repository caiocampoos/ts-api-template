
## Schemas

This diagram is only relevant for the current implementation of DB for this project, this might change along the way.

This project is developed in the bring your own database mindset, in the future this file will track the current implementation and use case.

<iframe width="560" height="315" src='https://dbdiagram.io/embed/63f2965f296d97641d822037'> </iframe>

### Current References

Doctors can have multiple appointments

Patients can have multiple appointments

Appointments need to have a doctor and a Patient

Appointments cannot be created with the same data and time


### Testing the Api locally


Download the files 

https://github.com/caiocampoos/nodejs-api-template/blob/main/docs/TS-API-TEMPLATE-POSTMAN-COLLECTION.json


and 

https://github.com/caiocampoos/nodejs-api-template/blob/main/docs/TS-API-TEMPLATE-POSTMAN-ENVIRONMENT.json


and import to postman.


Remember to select the correct enviroment TS Api Template Enviroment when using the collection.

Each folder of the collection tests one endpoint of the api locally(localhost:3001).

Start at Doctor endpoint create a doctor in the Create Doctor request, the pre-request script will generate the data for the test, no need to fill anything.

Next go to create Patient and do the same, you can create and delete Patients, the patient deleted will be the exat one created previously,
the scripts will fill the values for you, no need to worry.

The appointment secction the test scripts will fill the appointment with the last doctor created and last patient created, the only field you need to vary is the appointmentDate field.