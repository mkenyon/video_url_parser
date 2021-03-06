# VideoURLParser

Parse out information from a web video URL. Want information about a YouTube or
Facebook video?

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'video_url_parser'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install video_url_parser

## Usage

```ruby
VideoURLParser.parse('http://youtube.com/watch?v=5Qg6G7I4RS4#t=2m32s
# => { id: '5Qg6G7I4RS4', provider: :youtube }

VideoURLParser.parse('https://www.facebook.com/McLaren.Racing/videos/vb.12254981412/10153309389781413')
# => { id: '10153309389781413', provider: :facebook }

VideoURLParser.parse('https://example.com')
# => nil
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run
`rake` to run the tests. You can also run `bin/console` for an
interactive prompt that will allow you to experiment.

## Contributing

If you have a false negative, [I would love to hear
it](https://github.com/mkenyon/video_url_parser/issues/new).
If you would like support for other video providers,
please ask as well.

Bug reports and pull requests are welcome on GitHub at
https://github.com/mkenyon/video_url_parser.


## License

The gem is available as open source under the terms of the [MIT
License](http://opensource.org/licenses/MIT).

