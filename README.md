# stock_prices_python
# Stock prices
stock_prices = {
    "AAPL": 180,
    "TSLA": 250,
    "GOOGL": 130
}

total_investment = 0
while True:
    stock = input("Enter stock symbol (or type 'done' to finish): ").upper()
    if stock == 'DONE':
        break
    if stock in stock_prices:
        quantity = int(input(f"Enter quantity of {stock}: "))
        total_investment += stock_prices[stock] * quantity
    else:
        print("Stock not found!")

print("Total Investment: $", total_investment)
#this is stock prices python code.this code calculate the total investment by input stock prices. 
