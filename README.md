# base3
Reading Smart Contract Events on Base  Events allow you to track transfers, mints, swaps, and any on-chain activity.  Python example
event_filter = contract.events.Transfer.createFilter(fromBlock=12000000)
events = event_filter.get_all_entries()
print("Transfers:", len(events))
