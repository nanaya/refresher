fetcher: bundle exec sidekiq -c 40 -q feed_refresher_fetcher_critical,2 -q feed_refresher_fetcher -r ./app/boot.rb
parser: bundle exec sidekiq -c 1 -q feed_parser_$HOSTNAME -r ./app/boot.rb