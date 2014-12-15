# PaperTrail::Merge

*NOTE: WIP*

PaperTrail::Merge handles the case of merging changes from multiple 'branches'
of verions.  The original usecase was an offline application which needed to
synchronize potentially conflicting changes.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'paper_trail_merge'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install paper_trail_merge

## Usage

```ruby
post = Post.find(1)
post.merge_changes(version_starting_datetime, {title: "New title"})
```

## Contributing

1. Fork it ( https://github.com/btucker/paper_trail_merge/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
