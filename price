def find_best(prices):
    if not prices or len(prices) < 2:
        return None, None  

    min_price = prices[0]
    max_profit = 0
    buy_price = sell_price = prices[0]
    
    for price in prices[1:]:
        profit = price - min_price
        
        if profit > max_profit:
            max_profit = profit
            buy_price = min_price
            sell_price = price
            
        if price < min_price:
            min_price = price  

    return buy_price, sell_price  
    
prices = [5, 2, 1, 6, 9, 7]
buy, sell = find_best(prices)
print(f"Buy at {buy}, Sell at {sell}")
