# Instructions for use

Form.io provides access to private modules that contain premium components and themes for enterprise plans. In order to use them, you will need to be granted access and use the pkg.form.io registry to install the modules.

 - Ensure you have a form.io user account. Contact [support@form.io](mailto:support@form.io) and request access to private modules.
 - Go to https://pkg.form.io and log in with the username and password of your form.io account. Please note that this is the USERNAME and **not email** address of your account in form.io. You can access your username by logging into portal and going to your account information at the top right. If you are able to log in to https://pkg.form.io then you have been granted access and are using the correct username and password.
 - From within your project, log in to the package registry by running the following command:
   ```javascript
   npm adduser -r https://pkg.form.io
   ```
   Enter the same username and password from step 2.
 - Find the package you want to install in your app. Premium is a very common one. To install it, from the command line in your app.
   ```javascript
   npm install @formio/premium -r https://pkg.form.io
   ```
   This will install the package within your application.
 - To use it, in the main file of your app, Formio.use() the package. Depending on your language, do something like the following. (With react or vue, import Formio from react-formio or vue-formio instead of formiojs).
   ```javascript
   import { Formio } from 'formiojs';
   import premium from '@formio/premium';

   Formio.use(premium);
   ```
   Render forms as usual. Premium components will now be installed in your app.
