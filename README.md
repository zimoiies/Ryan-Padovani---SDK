# LordOfRings

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 14.2.8.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.


##Project Details


#MovieService
This TypeScript code file is part of an `Angular service` that manages HTTP requests to a movie-related API.

The service sends HTTP requests to the API using the **HttpClient** and **HttpHeaders** classes from the @angular/common/http package.


The base URL of the API is represented by the service's private property `endPoint(https://the-one-api.dev/v2/)`.

This Endpoint is only accessible through AccessToken which i get my signing in Lord Of Rings API
`Authorization = FOsnsTEuZWpAiYIBIvuw`

The HTTP headers for the requests made by the service are contained in an object called the httpOptions constant. The Authorization and Content-Type fields are found in the headers.

The basic URL of the API is accessed by the getAllMovies() method, which then returns the result. The get() method of the httpService receives the httpOptions headers as an argument from the method.

With the given movie ID, the getMovieById(id: number) method sends a GET request to the API and provides the response. The get() method of the httpService receives the httpOptions headers as an argument from the method.

With the given movie ID and an additional quote parameter in the URL, the searchMovies(id: number) function sends a GET request to the API to look for movie-related quotes. The get() method of the httpService receives the httpOptions headers as an input and delivers the result.


## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
