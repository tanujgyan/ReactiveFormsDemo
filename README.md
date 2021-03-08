This is a simple demo just aimed to show how to create reactive forms in Angular 11 and post the form data to .net core api which will then put in sql server\
There are 3 things we need to know to understand reactive forms
1. Form Control: This is the grassroot level element. This is used track value of controls and validate individual controls in a form
2. Form group: This is simply a collection of form controls
3. Form Builder: This is an injectable provider. its not necessary but it makes reactive forms easy

Steps 
1. Import ReactiveFormsModule in app module ts file
2. In your component class import FormBuilder,FormGroup and FormControl
3. In the html file the form should have an attribute [formGroup]. The name we give here will need to be initialized to new FormGroup in ts file. We can pass each formcontrol element inside the formGroup initialization. This is 2 way data binding
4. In the html file each element of the form like textbox or dropdown will have an attribute formControlName
