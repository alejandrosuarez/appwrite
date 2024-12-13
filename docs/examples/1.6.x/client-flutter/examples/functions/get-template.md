import 'package:appwrite/appwrite.dart';

Client client = Client()
    .setEndpoint('https://cloud.appwrite.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

Functions functions = Functions(client);

TemplateFunction result = await functions.getTemplate(
    templateId: '<TEMPLATE_ID>',
);