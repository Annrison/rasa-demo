## chitchat
* canthelp
    - utter_canthelp

## greet + canthelp
* greet
    - action_greet_user
* canthelp
    - utter_canthelp

## greet + newsletter + canthelp + continue
* greet
    - action_greet_user
* signup_newsletter
    - utter_can_do
    - subscribe_newsletter_form
    - form{"name": "subscribe_newsletter_form"}
* canthelp
    - utter_canthelp
    - utter_ask_continue_newsletter
* affirm
    - utter_great
    - subscribe_newsletter_form
    - form{"name": null}
    - utter_docu

## greet + newsletter + canthelp + don't continue
* greet
    - action_greet_user
* signup_newsletter
    - utter_can_do
    - subscribe_newsletter_form
    - form{"name": "subscribe_newsletter_form"}
* canthelp
    - utter_canthelp
    - utter_ask_continue_newsletter
* deny
    - utter_thumbsup
    - action_deactivate_form
    - form{"name": null}

## just sales + continue
* greet
    - action_greet_user
* contact_sales
    - utter_moreinformation
    - sales_form
    - form{"name": "sales_form"}
* canthelp
    - utter_canthelp
    - utter_ask_continue_sales
* affirm
    - utter_great
    - sales_form
    - form{"name": null}

## just sales + don't continue
* greet
    - action_greet_user
* contact_sales
    - utter_moreinformation
    - sales_form
    - form{"name": "sales_form"}
* canthelp
    - utter_canthelp
    - utter_ask_continue_sales
* deny
    - utter_thumbsup
    - action_deactivate_form
    - form{"name": null}

## Story from conversation with 541326c4cf36428dbd3ef5da1e80b0f7 on March 31st 2020

* greet
    - action_greet_user
    - slot{"shown_privacy":true}
* greet
    - action_greet_user
* ask_howdoing
    - action_chitchat
