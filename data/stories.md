## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## corona test safe
* corona_test
  - utter_symptoms
* deny
  - utter_had_any
* deny
  - utter_travel_14
* deny
  - utter_apply
* deny
  - utter_low_risk

## corona tracker path
* corona_state
  - action_corona_tracker

## interactive_story_1
* greet
    - utter_greet
* corona_test
    - utter_symptoms
* deny
    - utter_had_any
* deny
    - utter_travel_14
* deny
    - utter_apply
* deny
    - utter_low_risk
    - utter_greet
* corona_tracker
    - utter_state_name
* corona_state{"state": "karnataka"}
    - action_corona_tracker
* corona_state{"state": "punjab"}
    - action_corona_tracker
