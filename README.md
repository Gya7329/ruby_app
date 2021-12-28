# ruby_app
## Running Script

Navigate to directory where the script is located
```
$ cd /ruby_app
```

Run the script by passing in the name of the server logs you would like to parse

```
$ ruby ./parser.rb webserver.log
```

## Running Tests
Navigate to directory where the script is located
```
$ cd /ruby_app
```

Ensure rspec is installed by running
```
$ bundle install
```

Run tests by running
```
$ rspec spec/lib/logfile_parser_spec.rb
```


## Notes & Explanations


**CODE:**
- My approach was to take the simplest approach that could then be extended and improved upon.
- The first step was to decouple the code that does the parsing (`lib/logfile_parser.rb`) from the
script that calls it (`parser.rb`). This allows the parser (`lib/logfile_parser.rb`) to be reusable and can even be turned in to a gem.


