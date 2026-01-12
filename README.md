# 👋 Hi, I'm Angular Interview Hub

🚀 I create **Angular Interview Question Banks**  
🎯 Beginner → Advanced | Real Interview Questions

## 🧠 Topics Covered
- Angular Core
- TypeScript
- RxJS
- Signals
- Performance
- Testing

## 📘 Free Preview
👉 angular-interview-question-bank

## 🔐 Full Version (Paid)
💳 Premium Angular Interview Content  
👉 Buy here: ... comming soon...

## 📩 Contact
📧 rajubarse371@gmail.com
------------------------------------------------------------------------------------

------------------------------------------------------------------------------------
🚀 Angular Interview Question Bank

A curated collection of Angular interview questions and answers, covering Basic to Advanced concepts.
Designed for freshers, experienced developers, and interview preparation.

📘 BASIC ANGULAR QUESTIONS
1. What is the difference between Pure Pipes and Impure Pipes?

Answer:

Pure Pipes execute only when the input value changes.

Impure Pipes execute on every change detection cycle.

The async pipe is impure and automatically subscribes/unsubscribes to observables.

2. What are Standalone Components? How do you create them?

Answer:
Standalone components do not require NgModule. They were introduced in Angular 14.

Command:

ng generate component my-component --standalone

3. How do you bootstrap a Standalone Angular application?

Answer:
Use bootstrapApplication() in main.ts.

bootstrapApplication(AppComponent, {
  providers: [provideRouter(routes)]
});


Standalone routing uses loadComponent() instead of loadChildren().

4. What is APP_INITIALIZER in Angular?

Answer:
APP_INITIALIZER allows you to run logic before the application loads, such as:

Loading configuration

Authentication checks

App-level setup

5. What is trackBy in ngFor?

Answer:
trackBy improves performance by tracking list items using a unique identifier instead of re-rendering the entire list.

6. How do you reset a Reactive Form?

Answer:

this.myForm.reset();
this.myForm.updateValueAndValidity();

7. What is the difference between setValue() and patchValue()?

Answer:

setValue() → Requires all form controls

patchValue() → Allows partial updates

8. What is a Template-driven Form?

Answer:
Template-driven forms use directives like ngModel.
They are:

Easier to implement

Less scalable

Suitable for simple forms

9. What is Zone.js and how does it help Angular?

Answer:
Zone.js tracks async operations (events, promises, HTTP) and automatically triggers change detection in Angular.

10. What is router-outlet? Can we use multiple router outlets?

Answer:
Yes, using named router outlets.

<router-outlet name="sidebar"></router-outlet>


Routes must be configured with outlet property.

11. How do you handle errors in Observables? What is RxJS?

Answer:

Use catchError() for error handling

RxJS is a reactive programming library

Key operators:

forkJoin → Runs multiple observables in parallel

switchMap → Cancels previous observable

12. What are Directives in Angular?

Answer:

Component Directive

Structural Directive (*ngIf, *ngFor)

Attribute Directive (ngClass, ngStyle)

13. What are @HostListener and @HostBinding?

Answer:

@HostListener listens to host element events

@HostBinding binds properties to host element

14. What is angular.json?

Answer:
It is the Angular workspace configuration file.

Includes:

Build & serve configurations

Environment-specific settings

Assets and styles

15. How many ways can data be bound to the DOM?

Answer:

Interpolation

Property Binding

Event Binding

Two-way Binding

🚀 ADVANCED ANGULAR QUESTIONS
1. What improvements are available in the latest Angular versions?

Answer:

Standalone components

Signals

New control flow (@if, @for)

Better performance and tree-shaking

2. What is Tree Shaking?

Answer:
Tree shaking removes unused code during the build process to reduce bundle size.

3. How are services shared globally now?

Answer:
Using:

@Injectable({ providedIn: 'root' })


NgModule providers are no longer required.

4. What is a Reactive Form? How do you enable/disable fields?

Answer:

this.form.get('email')?.disable();
this.form.get('email')?.enable();

5. What is a Signal in Angular?

Answer:
Signals are reactive state primitives introduced in Angular 16 for fine-grained reactivity.

6. How do you create dynamic components?

Answer:
Using ViewContainerRef.createComponent().

7. How do you open a dynamic component in Angular Material Dialog?

Answer:

this.dialog.open(MyComponent);

8. Can we use multiple route guards? In what order do they run?

Answer:
Yes. Guards run left to right.

canActivate: [AuthGuard, RoleGuard, PermissionGuard]

9. How do you implement a global loader?

Answer:

Create a Loader Service

Use HTTP Interceptor to show/hide loader

10. How does HTML know when to stop the loader?

Answer:
HTML subscribes to a loader observable or signal exposed by the Loader Service.

11. What are @if, @for, @switch?

Answer:
New Angular 17+ control flow syntax, replacing *ngIf, *ngFor.

12. What are @defer, @viewport, @idle, @placeholder?

Answer:
They enable lazy loading UI blocks based on triggers like scroll, idle time, or interaction.

13. Signal Example: Button click counter (Even/Odd)

Answer:
Use signal() with computed() to derive even/odd state.

14. What is the purpose of spec.ts?

Answer:
Used for unit testing Angular components and services.

15. What frameworks are used for testing in Angular?

Answer:

Jasmine + Karma

Jest

Vitest

Cypress (E2E)

📌 Final Notes

✔ Real interview-focused
✔ Updated with latest Angular features
✔ Suitable for free preview or paid content
