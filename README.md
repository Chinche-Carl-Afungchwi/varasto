<!-- README.xml -->

<README>

<ProjectName>Varasto</ProjectName>

<Description>

Varasto is an inventory management system designed to help businesses manage their stock, sales, purchases, and expenses efficiently.

The application allows users to track product inventory, monitor sales trends, and generate reports to gain insights into business performance.

</Description>

<KeyFeatures>

<Feature>Product Management: Add, edit, and delete products with details such as price, stock quantity, and ratings.</Feature>

<Feature>Sales Tracking: Record sales transactions and monitor daily, weekly, or monthly sales summaries.</Feature>

<Feature>Expense Management: Track expenses across different categories and generate summaries.</Feature>

<Feature>Data Visualization: View charts for sales, purchases, and expenses for better decision-making.</Feature>

<Feature>Database Management: Manage data using PostgreSQL with Prisma ORM and Prisma Studio.</Feature>

</KeyFeatures>

<GettingStarted>

<Prerequisites>

<Requirement>Node.js: Ensure Node.js is installed on your machine (version >= 14.x).</Requirement>

<Requirement>PostgreSQL: Install PostgreSQL and ensure it is running.</Requirement>

<Requirement>Git: Required for cloning the repository.</Requirement>

</Prerequisites>

<Installation>

<Step>Clone the repository: git clone https://github.com/Chinche-Carl-Afungchwi/varasto.git</Step>

<Step>Navigate to the project directory: cd varasto</Step>

<Step>Install dependencies for the client and server: npm install</Step>

<Step>Create a .env file and configure environment variables as per the .env.example file.</Step>

<Step>Start the development server: npm run dev</Step>

</Installation>

</GettingStarted>

<ProjectStructure>

<Folder>client: Contains the frontend code built with Next.js.</Folder>

<Folder>server: Contains the backend code using Express and Prisma for the API.</Folder>

<Folder>src/state: Contains Redux Toolkit configuration and API slices.</Folder>

<Folder>src/app: Main Next.js pages and components for the client.</Folder>

</ProjectStructure>

<EnvironmentVariables>

<Variable>

<Key>DATABASE\_URL</Key>

<Description>Connection string for the PostgreSQL database.</Description>

</Variable>

<Variable>

<Key>NEXT\_PUBLIC\_API\_BASE\_URL</Key>

<Description>Base URL for connecting the frontend to the API.</Description>

</Variable>

</EnvironmentVariables>

<DatabaseSetup>

<Step>Ensure PostgreSQL is running and create a database named "varasto".</Step>

<Step>Update the DATABASE\_URL in the .env file with your PostgreSQL connection string.</Step>

<Step>Run migrations: npx prisma migrate dev --name init</Step>

<Step>Seed the database (if necessary): npm run seed</Step>

<Step>Use Prisma Studio to manage data: npx prisma studio</Step>

</DatabaseSetup>

<APIDocumentation>

<Endpoint>

<URL>/api/products</URL>

<Method>GET</Method>

<Description>Fetches a list of all products.</Description>

</Endpoint>

<Endpoint>

<URL>/api/sales</URL>

<Method>POST</Method>

<Description>Records a new sales transaction.</Description>

</Endpoint>

<Endpoint>

<URL>/api/expenses</URL>

<Method>GET</Method>

<Description>Fetches a list of all expenses with summaries.</Description>

</Endpoint>

</APIDocumentation>

<Testing>

<Strategy>

<Type>Unit Testing</Type>

<Description>Tested individual functions for adding products, fetching sales data, and calculating summaries.</Description>

</Strategy>

<Strategy>

<Type>Integration Testing</Type>

<Description>Tested interactions between API endpoints and database using real data.</Description>

</Strategy>

<Strategy>

<Type>System Testing</Type>

<Description>Ensured the entire system works together as expected on staging environments.</Description>

</Strategy>

<Strategy>

<Type>Acceptance Testing</Type>

<Description>Tested to ensure the software meets the business requirements and is ready for deployment.</Description>

</Strategy>

</Testing>

<Deployment>

<Platform>AWS Amplify</Platform>

<Details>

<Step>Configure AWS Amplify to connect with your GitHub repository.</Step>

<Step>Set environment variables in the Amplify console to match those in .env.</Step>

<Step>Deploy the frontend and backend by following Amplify's build and deploy steps.</Step>

</Details>

</Deployment>

<Contributing>

<Guideline>Fork the repository and create a new branch for your feature or bug fix.</Guideline>

<Guideline>Ensure your code follows the style guide and passes all tests.</Guideline>

<Guideline>Submit a pull request with a detailed description of your changes.</Guideline>

</Contributing>

<IssuesAndTroubleshooting>

<CommonIssue>

<Issue>Error: Can't reach database</Issue>

<Solution>Check that your DATABASE\_URL in the .env file is correct and the PostgreSQL server is running.</Solution>

</CommonIssue>

<CommonIssue>

<Issue>Build failed on AWS Amplify</Issue>

<Solution>Ensure that all environment variables are correctly set in the Amplify console and match those in .env.</Solution>

</CommonIssue>

</IssuesAndTroubleshooting>

<License>

<Type>MIT License</Type>

<Description>This project is licensed under the MIT License - see the LICENSE file for details.</Description>

</License>

</README>
