<div style="background-color:#09326C; color:white; padding:10px; display:flex; align-items:center; height:100%;">
  <h2 style="margin-top:4px; margin-bottom:4px; border-bottom:none; font-family:Arial;">
    <b>PayPal AI Migration Assistant PromptKit</b>
  </h2>
</div>

This Al PromptKit provides ready-to-use prompts for GitHub Copilot Chat to help you migrate from PayPal's legacy NVP/SOAP APIs to the modern REST APIs.

<h2 style="color:#09326C; font-family:Arial;">
  <b>Installation</b>
</h2>

1. Start by installing the VS Code Editor.
2. Visit the [VS Code extension marketplace](https://marketplace.visualstudio.com/vscode) or open the Extensions view in the VS Code Integrated Development Environment (IDE).
3. In the Extensions view, enter PayPal in the search bar.
4. Select "Install" to add the extension to your VS Code.
5. Once the extension is installed, click on the Paypal icon on the side navigation or tag <b>@paypal-migration-assistant<b> inside co-pilot chat to start AI migration feature.

<h2 style="color:#09326C; font-family:Arial;">
  <b>Migration Prompts Examples</b>
</h2>

1. **Convert Selected Code to PayPal REST API**

   - When to use: When you have a specific section of code using NVP/SOAP APIs that you want to convert to REST.
   - Instructions:

     - Select the code in your editor
     - Copy this prompt into GitHub Copilot Chat:

     ```
       Can you convert the selected code to its PayPal REST API equivalent?
     ```

2. **Understand Parameter Mapping**

   - When to use: When you need to understand how specific parameters map between NVP/SOAP and REST APIs.
   - Instructions:

     - Copy this prompt into GitHub Copilot Chat:

     ```
       What is parameter mapping with PayPal REST API?
     ```

     - If you want to have the mapping explained, use this prompt:

     ```
       For the selected NVP/SOAP code and the PayPal REST API,
       identify and explain the mapping of specific parameters between the two API styles.
     ```

       </div>

   - Pro tip: For mapping specific parameters, add the following to your query:

     - Copy this prompt into GitHub Copilot Chat:

     ```
       What is parameter mapping with PayPal REST API for PAYMENTREQUEST_0_AMT and PAYMENTREQUEST_0_CURRENCYCODE?
     ```

3. **Convert NVP/SOAP Payload to REST**

   - When to use: When you have a specific payload you want to convert to the REST format.
   - Instructions:

     - Select the NVP/SOAP payload in your editor or enter your payload in the chat
     - Copy this prompt into GitHub Copilot Chat:

     ```
       Given this NVP Payload, convert it to the equivalent JSON structure suitable for a REST API request.
     ```

4. **Convert Code with File Restructuring**

   - When to use: When converting larger sections of code that might benefit from being split into multiple files.
   - Instructions:

     - Select the code in your editor
     - Copy this prompt into GitHub Copilot Chat:

     ```
       Analyze the selected code section for potential modularization during its conversion to Paypal REST API.
       Identify logical components that could be separated into distinct files in the resulting RESTful implementation.
     ```

5. **Create REST API Client Class**

   - When to use: When you need a reusable REST API client class for your PayPal integration.
   - Instructions:

     - Copy this prompt into GitHub Copilot Chat:

     ```
       Generate a reusable client class in [language] for interacting with the PayPal REST API,
       including methods for payments and refunds.
       Ensure the class handles authentication, request formatting (JSON), and basic response handling.
     ```

6. **Add Error Handling for REST API**

   - When to use: When you need robust error handling for your REST API integration.
   - Instructions:

     - Select your REST API code (if any)
     - Copy this prompt into GitHub Copilot Chat:

     ```
       Can you enhance this code with comprehensive error handling for PayPal REST API calls?
     ```

<h2 style="color:#09326C; font-family:Arial;">
  <b>Common Migration Challenges and Solutions</b>
</h2>

- **Authentication**

  - NVP/SOAP uses API signatures, while REST uses OAuth 2.0.
  - Use this prompt:

    - Copy this prompt into GitHub Copilot Chat:

    ```
      Show me the step-by-step process and provide a code example in [language] for
      implementing PayPal REST API OAuth 2.0 authentication to replace my existing NVP/SOAP authentication method.
    ```

- **Sandbox Testing**

  - Use this prompt to update your sandbox testing approach:

    - Copy this prompt into GitHub Copilot Chat:

    ```
      Guide me through setting up a comprehensive PayPal REST API sandbox testing environment to replace my existing NVP/SOAP sandbox testing.
      Include steps for, but not limited to creating sandbox accounts, generating API credentials
      ([mention specific steps you want to include]), and verifying the behavior of my application with the new REST API
    ```

<h2 style="color:#09326C; font-family:Arial;">
  <b>Migration Best Practices</b>
</h2>

- Migrate incrementally - Convert one endpoint or feature at a time
- Maintain parallel implementations - Keep both API implementations running during transition
- Test thoroughly - Ensure each migrated component works correctly before proceeding
- Update documentation - Keep your internal documentation updated as you migrate
- Monitor errors - Pay close attention to error rates during and after migration

<h2 style="color:#09326C; font-family:Arial;">
  <b>Additional Resources</b>
</h2>

- [PayPal REST API Documentation](https://developer.paypal.com/api/rest/)
- [PayPal API GitHub Samples](https://github.com/paypal-examples)
