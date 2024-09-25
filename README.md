<img src="./readme/title1.svg"/>

<br><br>

<!-- project philosophy -->
<img src="./readme/title2.svg"/>

> Launchify is designed to provide startups with essential tools and strategies to achieve their business goals. By offering a comprehensive, data-driven platform, Launchify helps startups streamline processes, manage financial performance, connect with mentors, and secure investment opportunities. This holistic approach empowers startups to focus on innovation while receiving tailored support, ensuring a more efficient path to success. Through mentorship, financial analysis, and investment facilitation, Launchify fosters an environment where startups can thrive and reach their full potential

### User Stories

#### Startup

As a startup, I want to input my business data so I can receive tailored strategies to reach my goals.<br>
As a startup, I want to track my financial performance using the finance dashboard, so I can make informed decisions.<br>
As a startup, I want to request mentorship through the platform, so I can gain expert guidance and advice.<br>
As a startup, I want to provide detailed information about my investment needs, so I can attract potential investors.<br>

#### Investor

As an investor, I want to browse startup profiles and investment opportunities, so I can find projects that align with my interests.<br>
As an investor, I want to view detailed startup information, so I can make informed investment decisions.<br>

#### Mentor

As a mentor, I want to accept or decline mentoring requests, so I can manage my engagements with startups effectively.<br>
As a mentor, I want to offer advice and guidance to startups, so I can help them grow and succeed.

<br><br>

<!-- Tech stack -->
<img src="./readme/title3.svg"/>

### Launchify is built using the following technologies:

<li>This project uses the Laravel web development framework for the backend. Laravel is a robust PHP framework that provides powerful tools for building scalable and maintainable applications, with built-in support for routing, authentication, and database management.</li>
<li>For the database, Launchify uses MySQL, a reliable and widely-used relational database that ensures efficient data storage and retrieval, providing the platform with a solid foundation for managing startup, mentor, and investor information.</li>
<li>The frontend of the platform is built using React, a modern JavaScript library for building user interfaces. React allows for creating dynamic and responsive components that provide a seamless user experience across different devices.</li>
<li>For handling payments, Launchify integrates Stripe, a secure and scalable payment gateway that enables startups to manage transactions with ease and ensures investors can make safe, real-time investments.</li>
<li>To enable real-time communication features, Launchify uses WebSocket. This technology allows mentors and startups to engage in live chat sessions, enhancing communication and collaboration.</li>

<br><br>

<!-- UI UX -->
<img src="./readme/title4.svg"/>

> We designed Launchify using wireframes and mockups, refining the interface through multiple iterations to achieve an intuitive layout that ensures easy navigation and an optimal user experience.

- Project Figma design [figma](https://www.figma.com/design/OchjRDJIXGTsZvAcgiX8Jq/Platform-Startup-assistance?node-id=0-1&t=mNU2gk70JUhu0IVy-1)

<br><br>


### Mockups


| Home screen  |
| ---|
| ![Landing](./readme/Homepage.png) |

| Finance Dashboard  |
| ---|
| ![Dashboard](./readme/finance.png) |

<br><br>


<!-- Database Design -->
<img src="./readme/title5.svg"/>

### Architecting Data Excellence: Innovative Database Design Strategies:

- Insert ER Diagram here

<img src="./readme/ER-diagram.png" alt="database diagram"/>
<br><br>

<!-- Implementation -->
<img src="./readme/title6.svg"/>

### Admin Screens (Web)

|                              |                                 |                         |
| --------------------------------------------- | -------------------------------------------- | ------------------------------------------ |
|                |              |            |
| Startup Profile screen                        | Investor Profile Screen                      | MEntor Profile Screen                      |
| ![Landing](./readme/demo/Startup-Profile.jpg) | ![fsdaf](./readme/demo/Investor-Profile.jpg) | ![fsdaf](./readme/demo/Mentor-Profile.jpg) |

<br><br>

<!-- Prompt Engineering -->
<img src="./readme/title7.svg"/>

### AI-Driven Strategy Generation for Startups:

- The AI strategy generation function integrates with OpenAI's GPT model to create personalized business strategies for startups. It pulls data specific to each startup, such as industry, key challenges, and goals, to generate five actionable strategies following a structured format. Each strategy includes a name, description, action steps, and potential challenges. The AI request is securely made using the OpenAI API, and the generated strategies are parsed, stored in the database, and returned as a response to the user. This process ensures tailored and relevant strategic insights to address the startup's unique circumstances.

<br>

<img src="./readme/demo/Openai-startegies.png" alt="openai"/>

<br>

<!-- AWS Deployment -->
<img src="./readme/title8.svg"/>

### Efficient AI Deployment: Unleashing the Potential with AWS Integration:

- This project leverages AWS deployment strategies to seamlessly integrate and deploy natural language processing models. With a focus on scalability, reliability, and performance, we ensure that AI applications powered by these models deliver robust and responsive solutions for diverse use cases.

<br><br>

<!-- Unit Testing -->
<img src="./readme/title9.svg"/>

### Precision in Development: Harnessing the Power of Unit Testing:

- This project employs rigorous unit testing methodologies to ensure the reliability and accuracy of code components. By systematically evaluating individual units of the software, we guarantee a robust foundation, identifying and addressing potential issues early in the development process.

<img src="./readme/testing.png" alt="testing"/>

<br><br>

<!-- How to run -->
<img src="./readme/title10.svg"/>

> TTo set up Launchify locally, follow these steps:

### Prerequisites

Ensure that you have the following installed on your machine:

Node.js: <a href="https://nodejs.org/en"> Download Node.js</a><br>
Laravel: <a href="https://laravel.com/docs/11.x/installation"> Install Laravel</a><br>
Composer: <a href="https://getcomposer.org/download/"> Install Composer</a><br>
MySQL: <a href="https://www.mysql.com/downloads"> Download MySQL</a><br>

### Installation

1. Clone the repository

```sh
git clone https://github.com/Moussa-H/Launchify-Platform.git
cd Launchify-Platform
```

2. Create a .env file in the root of your Laravel project and add the following lines:

```sh
STRIPE_SECRET=sk_test_51Pyj3MFplAWf40dFgizow74eA027J0CJzbar5OyZc3nSmwJzOpCaEhhlvVNwrIu9htUdsmBmCsP3WvKBYAqYaPlQ00fYna4nCN
STRIPE_PUBLIC=pk_test_51Pyj3MFplAWf40dFg9WmvWgNbtyEBJ4DMqqKNIKM9bRswHgFQWLn7VqmVfd4LcJddFf2BfSHmjRQJY6bWYF4y7UQ00iAw5WP3j
BROADCAST_DRIVER=pusher
PUSHER_APP_ID=1865409
PUSHER_APP_KEY=a6d62ad7353778a90be9
PUSHER_APP_SECRET=18d4522271643cb868fa
PUSHER_APP_CLUSTER=eu
ML_SERVICE_URL=http://localhost:5000
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=db_launchify
DB_USERNAME=root

```

3. Run the migrations to set up the database:

```sh
php artisan migrate
```

4. Start the Laravel server:

```sh
php artisan serve
```

5. Navigate to the React frontend directory and install the dependencies:

```sh
cd frontend
npm install

```

Now you should be able to run Launchify locally and explore its features.
