$ gem install rest-client

irb
require 'rest-client'
URL = 'https... '
RestClient.get(URL)
response = RestClient.get(URL)
response.body

response = JSON.parse(RestClient.get(URL).body)
require 'json'
response.class
response.keys
response['results'].class
response['results'].first
response['results'].each{|char| puts char ['name'] }