# Response Area Template and Testing Sandbox

### Template Repository

[Response Area Template Repository](https://github.com/lambda-feedback-segp-sandbox/response-area-template) can be used to create and test new 
response areas. 

Template repository comes integrated with [Storybook](https://storybook.js.org/docs) module, 
via a custom addon.

### Getting started

1. To start, clone the repository by clicking [`Use this template`](https://github.com/lambda-feedback-segp-sandbox/response-area-template).<br><br>

2. Once cloned, navigate to the `components` folder, containing the following files:<br><br>

    1. `index.ts` contains the `MyResponseAreaTub` class. This class must extend the `ResponseAreaTub`, and contain two fields: `InputComponent` and `WizardComponent`.<br><br>

    2. `Input.component.tsx` contains the underlying function implementing `InputComponent` in `MyResponseAreaTub`.<br><br>

    3. `Wizard.component.tsx` contains the underlying function implementing `WizardComponent` in `MyResponseAreaTub`.<br><br>

3. Implement your response area by modifying the files listed above while not breaking the described requirements.

### Testing

To test a new response area, run the following commands:

1. Install the required dependencies:
```
$ yarn install
```

2. Run the Storybook application:
```
$ bash start_storybook
```
