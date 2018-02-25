# README


## Generate

### Channel
```
    rails generate channel Room
```

```
Running via Spring preloader in process 12787
      create  app/channels/room_channel.rb
   identical  app/assets/javascripts/cable.js
      create  app/assets/javascripts/channels/room.coffee
```

### Job
```
rails generate job MessageBroadcast
```

```
Running via Spring preloader in process 13125
      invoke  test_unit
      create    test/jobs/message_broadcast_job_test.rb
      create  app/jobs/message_broadcast_job.rb

```

### Model
```
    rails generate model Message content:string
```

```
Running via Spring preloader in process 13060
      invoke  active_record
      create    db/migrate/20180225120253_create_messages.rb
      create    app/models/message.rb
      invoke    test_unit
      create      test/models/message_test.rb
      create      test/fixtures/messages.yml
```

### Controller
```
    rails generate controller Rooms
```

```
Running via Spring preloader in process 13301
      create  app/controllers/rooms_controller.rb
      invoke  erb
      create    app/views/rooms
      invoke  test_unit
      create    test/controllers/rooms_controller_test.rb
      invoke  helper
      create    app/helpers/rooms_helper.rb
      invoke    test_unit
      invoke  assets
      invoke    coffee
      create      app/assets/javascripts/rooms.coffee
      invoke    scss
      create      app/assets/stylesheets/rooms.scss
```

### Views

views/messages/_message.html.erb
views/rooms/show.html.erb

## Config

### Routes
```ruby
Rails.application.routes.draw do
  root to: 'rooms#show'
end
```