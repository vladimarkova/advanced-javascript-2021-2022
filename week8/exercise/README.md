# Упражнение 8

1. Използвайки [Express](https://expressjs.com/) създайте сървър за базово менажиране на събития. Той да има следните endpoint-и:
    - **POST** /event, body: `{ name: string, capacity: number }` -- създава събитие и го връща в отговора;
    - **GET** /event/:id -- връща данните за дадено събитие;
    - **POST** /event/:id/book-spot, body: `{ firstName: string, lastName: string }` -- запазва дадения потребител в гостите на даденото събитие, ако има свободни места. В отговора да връща оставащите свободни места, ако е успяло да запази, в противен случай да връща грешка


   За запазвнето на местата използвайте [генератори](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Generator).