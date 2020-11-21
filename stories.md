## check in
*greet
  - utter_greet
*check_in_time
  - utter_check_in_time

## check out
*greet
  - utter_greet
*check_out_time
  - utter_check_out_time

## cancel reservation
*greet
  - utter_greet
*cancel_reservation
  - utter_cancel_reservation_1
  - utter_cancel_reservation_2

## cancellation policy
*greet
  - utter_greet
*cancellation_policy
  - utter_cancellation_policy

## restaurant_availability
*greet
  - utter_greet
*restaurant
  - utter_restaurant_availability

## restaurant timings
*greet
  - utter_greet
*restaurant_timings
  - utter_restaurant_timings

## breakfast_availability
*greet
  - utter_greet
*breakfast_availability
  - utter_breakfast_availability

## breakfast_timings
*greet
  - utter_greet
*breakfast_timings
  - utter_breakfast_timings

## direct check in
*check_in_time
  - utter_check_in_time

## direct check out
*check_out_time
  - utter_check_out_time

## direct cancel reservation
*cancel_reservation
  - utter_cancel_reservation_1
  - utter_cancel_reservation_2

## direct cancellation policy
*cancellation_policy
  - utter_cancellation_policy

## direct restaurant_availability
*restaurant
  - utter_restaurant_availability

## direct restaurant timings
*restaurant_timings
  - utter_restaurant_timings

## direct breakfast_availability
*breakfast_availability
  - utter_breakfast_availability

## direct breakfast timings
*breakfast_timings
  - utter_breakfast_timings

## happy path
*greet
  - utter_greet
*mood_great
  - utter_happy

## sad path 1
*greet
  - utter_greet
*mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
*affirm
  - utter_happy

## sad path 2
*greet
  - utter_greet
*mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
*deny
  - utter_goodbye

## book room number timings
*book_room {"timings" , "no_of_rooms" , "room_type"}
  - utter_room_booked
*thanks
  - utter_bye

## book room timings
*book_room {"timings"="tonight""}
  - utter_ask_no_of_room
*inform_rooms {"no_of_rooms"="2"}
  -utter_ask_room_type
*room_type {"room_type"="deluxe room"}
  - utter_room_booked
*thanks
  - utter_bye

## book room number
*book_room {"number" = "2"}
  - utter_ask_timings
*inform_time {"timings" = "tonight"}
  - utter_ask_room_type
* room_type{"room_type" = "deluxe room"}
  - utter_room_booked
*thanks
  - utter_bye

## book room
*book_room
  - utter_ask_no_of_room
*inform_rooms {"no_of_rooms" = "2"}
  - utter_ask_room_type
*room_type{"room_type" = "deluxe room"}
  - utter_ask_timings
*inform_time {"timings" = "tonight"}
  - utter_room_booked
*thanks
  - utter_bye

## clean room timings
*clean_room {"timings" = "right now"}
  - utter_confirm_cleaning

## clean room
*clean_room
  -utter_ask_timings
*inform_time {"timings" = "right now"}
  -utter_confirm_cleaning