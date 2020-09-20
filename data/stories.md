## happy path
* greet
  - utter_greet
* asking_for_restaurant_nearby
  - utter_ask_location
* location
  - action_set_location
  - slot{"location":"delhi"}
  - utter_ask_for_cusine
* cuisine
  - slot{"cuisine":"pizza"}
  - action_show_restaurant
  - utter_ask_booking_table
* booking_table

## sad path 1
* greet
  - utter_greet
* denying_restaurant finding
  - utter_cheer_up

## sad path 2
* greet
  - utter_greet
* un-understandable
    - utter_did_that_help

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot
