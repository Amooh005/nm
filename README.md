#def calculate_discount(price, discount_percent):
    """
    Calculate the final price after applying a discount.
    
    :param price: Original price of the item.
    :param discount_percent: Discount percentage.
    :return: Final price after discount if applicable, otherwise original price.
    """
    if discount_percent >= 20:
        return price - (price * discount_percent / 100)
    return price


original_price = float(input("Enter the original price of the item: "))
discount_percentage = float(input("Enter the discount percentage: "))


final_price = calculate_discount(original_price, discount_percentage)


print(f"Final price after discount: {final_price:.2f}")
 
