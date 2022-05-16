## React state management: Forms with input fields

1. Which of the following statements are true about the code snippet below? Pick two.

    ```js
    function ContactForm() {
      const [email, setEmail] = useState("");
      const handleEmailChange = (event) => setEmail(event.target.value);

      return (
        <form>
          <label htmlFor="name">
            Your name:
            <input
              id="name"
              type="text"
              name="name"

            />
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
      const [name, setName] = useState("");
      const [email, setEmail] = useState("");
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
    
    D. The `name` state variable gets updated as the user enters an input into the *name* field.
