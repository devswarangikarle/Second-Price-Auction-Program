# Second-Price-Auction-Program
In this task, you have to create a program for a special type of auction called a "second- price auction. " Here's how it works:  A number of people, say n, each secretly bid a certain amount of money. The person who bids the highest amount wins, but instead of paying their own bid, they pay the amount of the second- highest bid. 

n = int(input())
bids = list(map(int, input().split()))

max_bid = max(bids)
second_highest_bid = max(filter(lambda x: x < max_bid, bids))

winner_index = bids.index(max_bid) + 1

print(winner_index, second_highest_bid)
