# Coffee Ordering Form

Welcome to the **You Want Coffee** page! Here, you can place your coffee order by selecting your preferred coffee type and size. 

## How It Works

On this page, you’ll find a simple form where you can choose:

1. **Coffee Type:**
   - Espresso
   - Latte
   - Cappuccino
   - Americano

2. **Size:**
   - Small
   - Medium
   - Large

Once you've made your selections, click the **Order Coffee** button to submit your order.

## Form Details

The form submits a POST request to `/submit-coffee`. Here’s a breakdown of the form elements:

- **Coffee Type**: A dropdown menu allowing you to choose the type of coffee you want.
- **Size**: A dropdown menu for selecting the size of your coffee.
- **Submit Button**: A button to send your order.

### Example

Here’s an example of what the form looks like:

```html
<form action="/submit-coffee" method="post">
    <label for="coffee-type">Choose your coffee type:</label>
    <select id="coffee-type" name="coffee-type">
        <option value="espresso">Espresso</option>
        <option value="latte">Latte</option>
        <option value="cappuccino">Cappuccino</option>
        <option value="americano">Americano</option>
    </select>
    <br><br>
    <label for="size">Select size:</label>
    <select id="size" name="size">
        <option value="small">Small</option>
        <option value="medium">Medium</option>
        <option value="large">Large</option>
    </select>
    <br><br>
    <input type="submit" value="Order Coffee">
</form>
