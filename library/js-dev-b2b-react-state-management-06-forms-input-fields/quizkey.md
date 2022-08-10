## React state management: Forms with input fields

1. Which of the following statements are true about the code snippet below? Pick two.

   ```js
   function ContactForm() {
     const [email, setEmail] = useState('');
     const handleEmailChange = (event) => setEmail(event.target.value);

     return (
       <form>
         <label htmlFor="name">
           Your name:
           <input id="name" type="text" name="name" />
         </label>
         <label htmlFor="email">
           Your e-mail:
           <input
             id="email"
             type="email"
             name="email"
             onChange={handleEmailChange}
             value={email}
           />
         </label>
       </form>
     );
   }
   ```

   **Answers:** B and C

   B. The `email` field is being tracked by state.

   C. `event.target.value` references the contents of the email field.

2. Which of the following statements are true about the code snippet below? Pick two.

   ```js
   function SubscriberForm() {
     const [name, setName] = useState('');
     const [email, setEmail] = useState('');
     const handleNameChange = (event) => setName(event.target.value);
     const handleEmailChange = (event) => setEmail(event.target.value);
     return (
       <form>
         <label htmlFor="name">
           Enter Your Name:
           <input
             id="name"
             type="text"
             name="name"
             onChange={handleNameChange}
             value={name}
           />
         </label>
         <label htmlFor="email">
           Your Email:
           <input
             id="email"
             type="email"
             name="email"
             onChange={handleEmailChange}
             value={email}
           />
         </label>
       </form>
     );
   }
   ```

**Answers:** A and D

A. The `name` field is initialized to an empty string.
D. The `name` state variable gets updated as the user enters an input into the _name_ field.

3. True/False. A form input element is used to collect data in a HTML form.

A. True
B. False

**Answer: A**

4. True/False. An input element whose value is controlled by React state is called a controlled component.
   A. True
   B. False

**Answer: A**

5. True/False. Email is not a HTML input element type.
   A. True
   B. False

**Answer: B**

6. True/False. Keeping the input value in sync with React state makes it easier to handle the form data (such as submitting the data).
   A. True
   B. False

**Answer: A**

7. True/False. Text is not a HTML input element type.
   A. True
   B. False

**Answer: B**

8. True/False. You can use `<form>` tags to create a web-based HTML form.
   A. True
   B. False

**Answer: A**
