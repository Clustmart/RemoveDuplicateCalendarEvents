# Deduplicate Calendar Events

I use https://caldavsynchronizer.org to synchronise events from Outlook on Windows to my MacBook. Now there are cases where the Outlook entries are duplicated and synced to Macos. 
The solution I found with breyed/RemoveDuplicateCalendarEvents solves my problem, I had to tweak it a bit (remove event.hasRecurrenceRules from the if-condition as I want to include recurring events in the dedupe). I'm also planning to run the script recursively to keep my calendar clean.

## Usage

To show which calendar events would be removed, from Terminal run:

``` zsh
./rdce
```

To actually remove duplicate calendar events, from Terminal run:

``` zsh
./rdce --remove
```
