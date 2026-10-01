🔥 Technical Questions — VERY HIGH Probability
==============================================

### 3\. What is React Native?

**Answer:**

> “React Native is a framework for building mobile applications using JavaScript or TypeScript and React. It allows developers to create applications for platforms such as Android and iOS while sharing a significant amount of code between platforms.
> 
> Instead of developing the complete application separately for each platform, we can reuse components and business logic, which improves development efficiency.”

### 4\. React vs React Native?

React.jsReact NativeMainly for web applicationsMainly for mobile applicationsUses HTML elementsUses native mobile componentsRuns in browserRuns as a mobile applicationDOM is involvedUses native UI componentsWeb developmentAndroid/iOS development

**Interview answer:**

> “React.js is primarily used for building web interfaces, while React Native is used for building mobile applications. React.js works with web elements such as div and button, whereas React Native uses components such as View, Text and Pressable.”

### 5\. What is a component in React?

**Answer:**

> “A component is a reusable building block of a React application. It contains the UI and, depending on the component, its associated logic and state. Components make applications easier to maintain because we can divide a large interface into smaller reusable parts.”

### 6\. What is the difference between State and Props?

**Answer:**

> “Props are values passed from a parent component to a child component, whereas state is data managed inside a component.
> 
> Props are generally read-only from the receiving component's perspective, while state can change based on user actions or application logic.”

**Simple example:**

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   Props → Parent → Child  State → Data managed by the component itself   `

### 7\. What is useState?

**Answer:**

> “useState is a React Hook used to add and manage state in a functional component.”

Example:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   const [count, setCount] = useState(0);  setCount(count + 1);   `

Here count is the current state and setCount updates it.

### 8\. What is useEffect?

**Answer:**

> “useEffect is a React Hook used for side effects in a component. Examples include API calls, subscriptions, timers and interacting with external systems.
> 
> The dependency array determines when the effect runs.”

Example:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   useEffect(() => {    fetchUsers();  }, []);   `

With an empty dependency array, this effect runs after the component's initial render.

🚨 API Questions — VERY HIGH Probability
========================================

The job specifically mentions **REST APIs, JSON integration and API integration**, so prepare these extremely well.

### 9\. How do you integrate a REST API in React Native?

**Answer:**

> “I can integrate a REST API using either the Fetch API or a library such as Axios. I generally handle the loading, success and error states separately. I also parse the JSON response and update the component state with the received data.”

Example:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   const fetchUsers = async () => {    try {      setLoading(true);      const response = await fetch(API_URL);      const data = await response.json();      setUsers(data);    } catch (error) {      console.error(error);    } finally {      setLoading(false);    }  };   `

### 10\. What is REST API?

**Answer:**

> “REST stands for Representational State Transfer. A REST API allows applications to communicate through HTTP methods and resources.
> 
> Common methods are GET for retrieving data, POST for creating data, PUT or PATCH for updating data, and DELETE for deleting data.”

### 11\. GET vs POST?

**Answer:**

> “GET is generally used to retrieve data from the server, while POST is generally used to send data to the server and create a new resource.”

### 12\. What is JSON?

**Answer:**

> “JSON stands for JavaScript Object Notation. It is a lightweight format commonly used to exchange data between a client application and a server.”

Example:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   {    "name": "Rahul",    "age": 22  }   `

### 13\. What happens if an API fails?

**Answer:**

> “I would handle the error using try-catch or appropriate error handling. I would check the HTTP status, log the error during development, show an appropriate message to the user and make sure the application doesn't crash. Depending on the API, I may also implement retry or fallback behavior.”

🧠 JavaScript Questions
=======================

### 14\. Difference between var, let and const?

**Answer:**

> “var is function-scoped, while let and const are block-scoped. let allows reassignment, whereas const does not allow reassignment of the variable binding. In modern JavaScript, I generally prefer const by default and use let when reassignment is required.”

### 15\. What is a Promise?

**Answer:**

> “A Promise represents the eventual completion or failure of an asynchronous operation. It can be in pending, fulfilled or rejected state.”

### 16\. What is async/await?

**Answer:**

> “async/await is syntax built on top of Promises that makes asynchronous JavaScript code easier to read and maintain.”

Example:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   const getData = async () => {    try {      const response = await fetch(API_URL);      const data = await response.json();      return data;    } catch (error) {      console.error(error);    }  };   `

### 17\. What is the difference between == and ===?

**Answer:**

> “== performs type coercion before comparison, while === checks both value and type without implicit type conversion. I generally prefer === because it provides more predictable comparisons.”

📱 React Native Questions
=========================

### 18\. What are common React Native components?

**Answer:**

> “Some commonly used components are View, Text, Image, TextInput, Pressable, ScrollView, FlatList and ActivityIndicator.”

### 19\. ScrollView vs FlatList?

**Answer:**

> “ScrollView renders its content together, so it can become inefficient for very large lists. FlatList is designed for lists and renders items more efficiently using virtualization. For large or dynamic lists, I would generally prefer FlatList.”

### 20\. How would you improve React Native app performance?

**Answer:**

> “I would first identify the actual bottleneck using profiling and debugging tools. Depending on the problem, I could optimize unnecessary re-renders, use FlatList for large lists, optimize images, reduce unnecessary API calls, memoize expensive computations or components where appropriate, and avoid unnecessary state updates.”

This is particularly relevant because the job explicitly mentions resolving **bugs and performance issues**.

🗺️ Google Maps API — Prepare This
==================================

The job explicitly lists **Google Maps API** as a required skill.

### 21\. Have you worked with Google Maps API?

If **YES**:

> “Yes. I have used Google Maps integration to display maps and locations. I understand concepts such as markers, coordinates, map regions and location-based interactions. I can also integrate location data received from an API into the map.”

If **NO**, **don't lie**.

Say:

> “I haven't implemented it in a production project yet, but I understand the basic concepts and I have worked with APIs and React Native. I’m confident I can integrate Google Maps by following the documentation and handling API keys, permissions, coordinates and markers correctly.”

That is much safer than pretending.

🐛 Debugging Questions
======================

### 22\. Your app crashes. What will you do?

**Strong answer:**

> “First, I would reproduce the issue consistently. Then I would check the error message and stack trace, identify the component or function causing the problem, and inspect the relevant state, props and API responses.
> 
> I would isolate the root cause, fix it, test the affected functionality and then test related functionality to make sure the fix hasn't introduced another issue.”

### 23\. API data is not showing on the screen. How do you debug it?

**Answer:**

> “I would check it step by step:
> 
> 1.  Verify that the API request is actually being sent.
>     
> 2.  Check the URL, parameters and headers.
>     
> 3.  Check the HTTP status code.
>     
> 4.  Log the response.
>     
> 5.  Verify the JSON structure.
>     
> 6.  Check whether the state is being updated.
>     
> 7.  Check whether the UI is reading the correct property.
>     
> 8.  Handle loading and error states.”
>     

This type of **practical troubleshooting question is very likely** for this role.

🔀 Git Questions
================

### 24\. What is Git?

**Answer:**

> “Git is a distributed version control system used to track code changes and collaborate with other developers.”

### 25\. What Git commands do you know?

Be ready to explain:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   git clone  git status  git add  git commit  git push  git pull  git branch  git checkout  git merge   `

Don't just memorize commands. Know what each does.

### 26\. What is a Git branch?

**Answer:**

> “A branch allows us to work on a separate line of development without directly affecting the main branch. For example, I could create a feature branch, develop and test the feature, and then merge it into the main branch after review.”

🏗️ Existing Codebase Question
==============================

This one is particularly important because the JD specifically says candidates should be able to **work with existing codebases**.

### 27\. You are given an unfamiliar existing project. What will you do?

**Excellent answer:**

> “First, I would understand how the project is structured and how it is built and run. Then I would identify the main entry points, navigation, components, state management, API layer and configuration.
> 
> I would run the application and understand the existing functionality before making changes. Then I would trace the specific feature or bug through the relevant files, make a small change, test it and gradually understand more of the codebase.
> 
> I would avoid making unnecessary changes to code I don't yet understand.”

That answer shows **engineering maturity**.

👨‍💼 HR Questions
==================

### 28\. Why should we hire you?

**Answer:**

> “I believe I can contribute because I have the technical foundation required for this role and I’m comfortable learning quickly. I understand React, React Native, JavaScript, APIs and Git, and I enjoy solving practical development problems.
> 
> I also understand that this role requires working with existing code, debugging issues and collaborating with developers and designers. I’m willing to take ownership of my tasks, learn from feedback and continuously improve.”

### 29\. What are your strengths?

Choose **2–3 genuine strengths**, for example:

> “My main strengths are problem-solving, willingness to learn and persistence when debugging technical issues. I also try to understand the root cause instead of applying a temporary fix.”

### 30\. What is your weakness?

Avoid:

❌ “I am a perfectionist.”

Better:

> “Earlier, I sometimes spent too much time trying to solve a problem independently before asking for help. I've been improving this by first investigating systematically and then asking a focused question when I’m blocked, along with explaining what I’ve already tried.”

### 31\. Where do you see yourself in 3–5 years?

**Answer:**

> “I want to become a strong full-stack or mobile-focused developer who can independently handle features from understanding requirements through development, API integration, testing and deployment. I also want to gradually take more responsibility for technical decisions and mentoring.”

💰 32. What are your salary expectations?
=========================================

The posted salary range is **₹10,000–₹15,000**, so don't give an expectation wildly outside the advertised range.

**Safe answer:**

> “I understand that the role has a stated range of ₹10,000 to ₹15,000. Considering the role, responsibilities and my skills, I would be comfortable discussing compensation within that range. My primary focus is also getting good practical experience and contributing to the team.”

⚠️ Questions I Would Expect Them to Ask From Your Project
=========================================================

This is where many freshers lose interviews.

If you put **any project on your resume**, expect:

1.  **Explain your project.**
    
2.  Why did you choose this technology?
    
3.  What exactly was your contribution?
    
4.  What was the hardest problem you faced?
    
5.  How did you solve it?
    
6.  Did you integrate an API?
    
7.  Which API did you use?
    
8.  How did you handle API errors?
    
9.  How did you manage state?
    
10.  How did you test the application?
    
11.  How did you debug it?
    
12.  What would you improve if you had more time?
    
13.  Did you use Git?
    
14.  How did you structure your project?
    
15.  **Show us the project/code.**
    

### 🚨 Most important rule

**Know every line of the project you put on your resume.**

If you write:

> “Implemented Google Maps API”

they can immediately ask:

> “How did you implement it?”

If you write:

> “REST API integration”

they can ask:

> “Show me the API call.”

If you write:

> “React Native application”

they can ask:

> “Why React Native instead of native Android?”

So don't memorize only definitions. **Prepare to explain your actual projects technically.**

🔥 My Top 15 to Prepare First
=============================

If your interview is very soon, prioritize these:

PriorityQuestion🔴 1Tell me about yourself🔴 2Explain your project🔴 3React vs React Native🔴 4How do you integrate REST API?🔴 5Explain useState🔴 6Explain useEffect🔴 7Props vs State🔴 8GET vs POST🔴 9How do you debug an API issue?🔴 10ScrollView vs FlatList🔴 11JavaScript let, const, var🔴 12Promise / async-await🔴 13Git basics🔴 14Google Maps API🔴 15Why should we hire you?
