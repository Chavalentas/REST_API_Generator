# REST_API_Generator
**YOU DO NOT HAVE TO PROGRAM A REST-API ANYMORE! GENERATE IT!**
</br>
This is a big project that demonstrates my skills in frontend (TypeScript, Angular, HTML, SASS) and
backend development (JavaScript, Node-RED).
It is a useful client-server application that can facilitate backend development by
automatically generating REST-API configurations that can be easily deployed in Node-RED 
(either automatically or manually).
The REST-API generator supports two RDBMS: 
* Microsoft SQL Server
* PostgreSQL

Refer to [the screenshot guide](#screenshot-guide) for more information.

## Used technologies
![Angular](https://img.shields.io/badge/angular-%23eb4034?style=for-the-badge&logo=angular)
![TypeScript](https://shields.io/badge/TypeScript-3178C6?logo=TypeScript&logoColor=FFF&style=for-the-badge)
![HTML](https://img.shields.io/badge/html-%23d4b655?style=for-the-badge&logo=html5)
![SASS](https://img.shields.io/badge/sass-pink?style=for-the-badge&logo=sass)
![Node-RED](https://img.shields.io/badge/node--red-%23120201?style=for-the-badge&logo=node-red)
![JavaScript](https://img.shields.io/badge/javascript-yellow?style=for-the-badge&logo=javascript)

* **Frontend:** Angular
* **Backend:** Node-RED

## Generator architecture
![Generator](img/prototype_node_red_drawing.png)

## <a name="screenshot-guide"></a>Screenshot guide
**Step 1:** Open Node-RED in the command line.
</br>
![Step1](img/step1.png)
</br>
**Step 2:** Import the necessary flows that are part of the backend application.
</br>
![Step2](img/step2.png)
</br>
**Step 3:** Import the [Schema-Parser](./Node-RED-Flows/Schema_Parser_Flow/schema_parser.json)
and the [REST-API-Generator](./Node-RED-Flows/Config_Generator_Flow/config_generator_service.json).
</br>
![Step3](img/step3.png)
</br>
**Step 4:** Deploy the both flows (start the backend application).
</br>
![Step4](img/step4.png)
</br>
**Step 5:** Start the [Angular frontend application](./Frontend/prototype-frontend) using **ng serve** in your
command line. Configure all necessary information [here](./Frontend/prototype-frontend/src/app/configuration).
</br>
**Step 6:** Enter the database data about the database your REST-API relies upon.
</br>
![Step5](img/step5.png)
</br>
**Step 7:** Select the database schema.
</br>
![Step6](img/step6.png)
</br>
**Step 8:** Select the object type (table, view, function or stored procedure).
</br>
![Step7](img/step7.png)
</br>
**Step 9:** Select the object name.
</br>
![Step8](img/step8.png)
</br>
**Step 10:** Select the REST-API name (is displayed in the Node-RED tab).
</br>
![Step9](img/step9.png)
</br>
**Step 11:** Copy the JSON-configuration of the REST-API flow
</br>
![Step10](img/step10.png)
</br>
and paste in the flow import manually.
</br>
![Step11](img/step11.png)
</br>
Deploy the flow manually.
</br>
![Step12](img/step12.png)
</br>
**OR**
</br>
Import the flow automatically.
</br>
![Step14](img/step14.png)
</br>
Enter the URL of the Node-RED instance where the REST-API should be deployed.
</br>
![Step15](img/step15.png)
</br>
You will receive a notification that the flow was succesfully imported and deployed.
</br>
![Step16](img/step16.png)
</br>
As you can see, the flow is deployed automatically.
</br>
![Step17](img/step17.png)
</br>
**Step 12:** Test the deployed REST-API (tested with Postman). It works!
</br>
![Step13](img/step13.png)