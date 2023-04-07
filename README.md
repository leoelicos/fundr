# Fundr

![Node.js](https://img.shields.io/badge/16.15.0%20LTS-0?label=Node.js&style=for-the-badge&labelColor=white&color=black) ![Express.js](https://img.shields.io/badge/4.17.1-0?label=Express&style=for-the-badge&labelColor=white&color=black) ![Mysql2](https://img.shields.io/badge/2.2.1-0?label=Mysql2&style=for-the-badge&labelColor=white&color=black) ![Sequelize](https://img.shields.io/badge/6.3.5-0?label=Sequelize&style=for-the-badge&labelColor=white&color=black) ![dotenv](https://img.shields.io/badge/8.2.0-0?label=dotenv&style=for-the-badge&labelColor=white&color=black) ![bcrypt](https://img.shields.io/badge/5.0.0-0?label=bcrypt&style=for-the-badge&labelColor=white&color=black) ![express-handlebars](https://img.shields.io/badge/5.2.0-0?label=express-handlebars&style=for-the-badge&labelColor=white&color=black) ![express-session](https://img.shields.io/badge/1.17.1-0?label=express-session&style=for-the-badge&labelColor=white&color=black) ![connect-session-sequelize](https://img.shields.io/badge/7.0.4-0?label=connect-session-sequelize&style=for-the-badge&labelColor=white&color=black) ![eslint](https://img.shields.io/badge/7.0.4-0?label=eslint&style=for-the-badge&labelColor=white&color=black) ![prettier](https://img.shields.io/badge/2.1.2-0?label=prettier&style=for-the-badge&labelColor=white&color=black)

## Introduction

Fundr allows users to view and create crowdfunding projects. It follows the MVC model and uses `Handlebars.js`, `Sequelize`, `Express.js`, and `Node.js`.

The app uses `Handlebars.js` to render the data from the back end to the front end, and `mysql2` to handle the database.

It also facilitates login/logout capability using `express-session`.

I made this app to learn about `handlebars` including `layouts` and `partials`, and also the `Model-View-Controller` modularization.

Deployed API: https://fundr.herokuapp.com/api/

## Installation

| Steps                             | Details                                                                         |
| --------------------------------- | ------------------------------------------------------------------------------- |
| Install `Node.js `                | https://nodejs.org/en/                                                          |
| Install `Mysql`                   | https://dev.mysql.com/downloads/installer/                                      |
| Install `Insomnia`                | https://insomnia.rest/download                                                  |
| Clone this repo                   | `git clone`<br>https://github.com/leoelicos/fundr.git                           |
| Go inside                         | ` cd fundr`                                                                     |
| Rename `.env.EXAMPLE`             | ` mv .env.Example .env`                                                         |
| Input mysql credentials in `.env` | ` DB_USER={username}`<br>`DB_PW={password}`<br>_Don't forget to save the file!_ |
| Initialize database               | `cd db`<br>`mysql -u root -p`<br>`{password}`<br>`source schema.sql;`<br>`exit` |
| Install dependencies              | `cd ..`<br>`npm install`                                                        |
| Run seeds                         | `npm run seed`                                                                  |

## Usage

### Insomnia

| Steps                                          | Details                            |
| ---------------------------------------------- | ---------------------------------- |
| Start the server                               | `npm start`                        |
| Root endpoint                                  | GET `localhost:3001`               |
| Search all projects                            | GET `/`                            |
| Find a specific project                        | GET `/project/:id`                 |
| Form to log in / create account                | GET `/login`                       |
| See user's projects and form to create project | GET `/profile`                     |
| If already logged in, be redirected            | GET `/login` > redirect `/profile` |

## Video Demo

Test

## Screenshots

### Screenshot: Test

![Test](Test)

## Credits

- BCS Resources

## License

&copy; Leo Wong <leoelicos@gmail.com>

Licensed under the [MIT License](./LICENSE).
