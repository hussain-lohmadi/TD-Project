# DZASHA SHOPPING APP
![UI IMAGE](https://github.com/user-attachments/assets/08c0bd17-137c-47cd-a6f8-2edb2c968f81)
DZASHA
## Key Features
- **Product Details**
  
         Detailed product descriptions, including materials, care instructions, and size guides.
- **Shopping Cart**
  
        Users can add products to their cart for later purchase.
- **Checkout Process**
  
       Allow users to make purchases without creating an account.
- **Order Tracking**

        Users can view their past orders and track current shipments.
- **Wishlist**
  
        Users can save items they like for future purchase.

---
## Installation Guide
### For Windows:
 1. Locate the downloaded file (e.g., `FocusProSetup.exe`) in your **Downloads** folder
 2. Double-click the file to start the installation
   
 3. Follow the on-screen instructions, and select:
     - Installation Folder (default is usually fine)
     - Create a Desktop Shortcut (optional)
 4. Click “**Install**” and wait for the installation to complete.
 
 5. Once finished, click “**Finish**” to launch the app

### For macOS
 1. Locate the downloaded file (e.g., `FocusPro.dmg`) in your **Downloads** folder
 
 2. Double-click the file to open the installation window
 
 3. Drag the "**FocusPro**" icon into the Applications folder 
 
 4. Open the Applications folder and double-click "**FocusPro**" to launch the app  

### For linux 
  1. Locate the downloaded file (e.g., `FocusPro.tar.gz` or `FocusPro.deb`) in your **Downloads** folder
   
  2. Open a terminal window
   
  - For `.deb` Package (Ubuntu, Debian[^3]):
     ```bash
     cd ~/Downloads
     sudo dpkg -i FocusPro.deb
     ```
     - If any dependencies are missing, fix them with:
       ```bash
       sudo apt-get install -f
       ```
  
  - For `.tar.gz` Package (General Linux[^3]):
     ```bash
     cd ~/Downloads
     tar -xvzf FocusPro.tar.gz
     cd FocusPro
     ./install.sh
     ```
    - Follow any on-screen instructions provided by the installation script
---   
## User Guide
### Creating an Account
- [x] **Sign Up**:   
      1. Tap on the Sign Up button on the home screen.   
      2. Fill in the required fields: name, email, password, and phone number.   
      3. Accept the terms and conditions, then tap Create Account.
- [x] **Log In**:   
      1. If you already have an account, tap on Log In.   
      2. Enter your email and password, then tap Log In.
- [x] **Social Media Login**:      
       You can also log in using your Google or Facebook account.
### Searching for Products   
- [x] **Search Bar**:      
       Use the search bar at the top of the screen to enter keywords (e.g., "jeans," "t-shirts").
- [x] **Filters**:      
      Apply filters for size, color, price range, and brand to narrow down your search results.
### Viewing Product Details
- [x] **Select a Product**:      
       Tap on a product image from the list to view its details.
- [x] **Product Information**:      
      Check out high-quality images, descriptions, size guides, and customer reviews.
- [x] **Size and Fit**:      
       Refer to the size chart provided for accurate fitting.
### Checking Out
- [x] **Proceed to Checkout**:      
      Once you're ready, tap on Checkout in your cart.
- [x] **Shipping Information**:      
      Enter your shipping address and select your preferred shipping method.
- [X] **Payment Options**:   
       Choose your payment method (credit card, PayPal, etc.) and enter the necessary details.
- [X] **Complete Purchase**:   
       Tap on Place Order to finalize your purchase.
### Customer Support     
  - In case, facing any problem; you can contact support team[^1].
## Collaboration

DZASHA collaborated with many payment companies, to make the experience more flixible

| Company          | Country of Origin | Established | Key Services                                     | Notable Partnerships        |
|-------------------|------------------|-------------|--------------------------------------------------|------------------------------|
| PayPal            | USA              | 1998        | Online payments, money transfers, invoicing      | eBay, Shopify                |
| Stripe            | USA              | 2010        | Payment processing, subscription billing          | Amazon, Lyft                 |
| Square            | USA              | 2009        | Point of sale, online payments, invoicing        | Weebly, QuickBooks           |
| Adyen             | Netherlands      | 2006        | Global payment processing, risk management        | Uber, Spotify                |
| Payoneer          | USA              | 2005        | International payments, cross-border transactions | Upwork, Fiverr               |
| Revolut           | UK               | 2015        | Banking services, international money transfers   | Mastercard                   |
| Worldpay          | UK               | 1989        | Payment processing, fraud protection              | Visa, American Express       |
| Braintree         | USA              | 2007        | Mobile and web payment systems                    | Uber, Airbnb                 |
| Klarna            | Sweden           | 2005        | Buy now, pay later, payment processing            | H&M, Expedia                 |
| Zelle             | USA              | 2017        | Instant money transfers between bank accounts     | Bank of America, Chase       |


---
## Troubleshooting

Here are some common issues users might encounter while using DZASHA

- **Payment Declined**
  - ***Definition***:  
    Insufficient funds, incorrect card details, or the card issuer blocking the transaction.
  - ***Solution***:  
    - Check your bank account balance.
    - Verify that your card number, expiration date, and CVV are entered correctly.
    - Contact your bank or card issuer for assistance.
- **Issue: Transaction Timeout**
  - ***Definition***:  
   Slow internet connection or server issues.
   - ***Solution***:  
     - Ensure you have a stable internet connection.
     - Try refreshing the page or restarting the app.
     - If the problem persists, wait a few minutes and try again.

- **Issue: Account Locked**
   - ***Definition***:  
   Multiple failed login attempts may lead to account lockout for security reasons.
  - ***Solution***:  
     - Wait for a set period (e.g., 15 minutes) before trying to log in again.
     - If you cannot log in after waiting, use the “Forgot Password?” option to reset your credentials.

For further assistance, please refer to the support section or contact customer support[^1].

--- 

## Advanced Usage

### How to add your product in DZASHA

- **Accessing the Seller Dashboard**:
   - Log in to your account and navigate to the seller dashboard from the profile menu.
   - Familiarize yourself with the dashboard layout, including sections for products, orders, and analytics.
      - Benefits :
        A centralized location for managing all aspects of your product listings and sales.

- **Adding a New Product**:
   - How to Use:
      1. Click on the “Add Product” button in the seller dashboard.
      2. Fill in the required fields, including product name, category, and brand.
      3. Click “Save” to add the product to your inventory. 

- **Adding Image**:
   - after adding your product, you can embed an image at the HTML section
     ```html
     <img src="URL_TO_IMAGE" alt="Product Image" width="300" height="400">
     ```

- **Save Your Product**:
   - Once you are satisfied with the results, save it and set a price for it.

### Example Script

Below is a simple example script that adds your product.

```java
import java.io.OutputStream;
import java.net.HttpURLConnection;
import java.net.URL;
import java.nio.charset.StandardCharsets;

public class AddProductExample {

    public static void main(String[] args) {
        try {
            // URL of the API endpoint for adding a product
            URL url = new URL("https://yourapi.com/api/products");

            // Creating an HTTP connection
            HttpURLConnection connection = (HttpURLConnection) url.openConnection();
            connection.setRequestMethod("POST");
            connection.setRequestProperty("Content-Type", "application/json; utf-8");
            connection.setRequestProperty("Accept", "application/json");
            connection.setDoOutput(true);

            // Product data to be sent in JSON format
            String jsonInputString = """
                {
                    "productName": "Classic Denim Jacket",
                    "category": "Jackets",
                    "brand": "Your Brand",
                    "price": 79.99,
                    "description": "A classic denim jacket made from 100% organic cotton.",
                    "sizes": ["S", "M", "L", "XL"],
                    "colors": ["Light Blue", "Dark Blue"],
                    "stock": 100,
                    "imageUrl": "https://yourimageurl.com/denim-jacket.jpg"
                }
                """;

            // Writing the JSON input to the request body
            try (OutputStream os = connection.getOutputStream()) {
                byte[] input = jsonInputString.getBytes(StandardCharsets.UTF_8);
                os.write(input, 0, input.length);
            }

            // Reading the API response
            int responseCode = connection.getResponseCode();
            if (responseCode == HttpURLConnection.HTTP_CREATED) {
                System.out.println("Product added successfully!");
            } else {
                System.out.println("Failed to add product. Response Code: " + responseCode);
            }

            // Closing the connection
            connection.disconnect();

        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}

```

# FOOTNOTES
[^1]:
### to contact us:
S444001990@UQU.EDU.SA


[^3]:
### more infos about the difference between **Ubuntu** and **General Linux** 
- Linux is a broad term that encompasses all operating systems built around the Linux kernel.
- Ubuntu is a specific user-friendly Linux distribution derived from Debian, designed to be accessible and widely supported.
In essence, Ubuntu is a Linux distribution, but not all Linux distributions are Ubuntu. Ubuntu takes the Linux kernel and adds its own customizations, software, desktop environment, and tools to create a cohesive operating system.
