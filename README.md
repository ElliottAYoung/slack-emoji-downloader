# Slack Emoji Downloader
This is a simple Ruby script to download all of the emojis from a given Slack Team and place them into a directory for you to use.

Using the script is simple, there is only one step for setup, simply change line #5 in `runner.rb` from `"your-slack-token"` to whatever your Slack API token is for that team.

Once you've done that simply run the script with the command

```
$ ruby runner.rb
```

It will output all emojis to the newly created `images` directory.

## Dependencies

Of the three libraries this script needs to work only one of them, HTTParty, is not incldued in default ruby. It's a simple HTTP Client, download it with the following:

```
$ gem install httparty
```

## Uploding Emojis to a Slack Team
Only loosely related to this script, if you want to upload all of your emojis to a different slack team and dont want to do it by hand I recommend using [This Chrome Extension](https://chrome.google.com/webstore/detail/slack-emoji-tools/anchoacphlfbdomdlomnbbfhcmcdmjej?hl=en) to bulk upload all of them.
