# Deduplicate Calendar Events

I use https://caldavsynchronizer.org to synchronise events from Outlook on Windows to my MacBook. Now there are cases where the Outlook entries are duplicated and synced to Macos. 

The solution I found with breyed/RemoveDuplicateCalendarEvents did inspire me to solves my problem, I had to tweak it a bit (as redefining the UniqueEventIdentifier based on startDate and title) as I needed also for recursive events. 

## Usage

To show which calendar events would be removed, from Terminal run:

``` zsh
./rdce
```

To actually remove duplicate calendar events, from Terminal run:

``` zsh
./rdce --remove
```
