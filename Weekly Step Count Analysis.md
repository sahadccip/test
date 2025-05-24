# Weekly Step Count Analysis

##  Welcome to an imaginary analysis of how many steps I walked each day for a week, compared with my friends.

**Daily step counts**

*track your health along with wealth so that you can enjoy*

~~kill your laziness like strike through~~

`<p> The more the steps the more the bosy wealth</p>`

```erlang
   -module(steps_simple).
-export([my_steps/0, friends_steps/0, compare_steps/0]).

% Your steps for two days (Mon and Tue)
my_steps() ->
    [6000, 7500].

% Steps for two friends
% Format: [{FriendName, [Mon, Tue]}]
friends_steps() ->
    [
        {"Sahad", [7000, 8000]},
        {"Sneha",   [5000, 7200]}
    ].

% Compare your total steps with each friend
compare_steps() ->
    MyTotal = lists:sum(my_steps()),
    io:format("Your total steps: ~p~n", [MyTotal]),

    lists:foreach(fun({Name, Steps}) ->
        Total = lists:sum(Steps),
        Comparison =
            case Total of
                _ when Total > MyTotal -> "more than you";
                _ when Total < MyTotal -> "less than you";
                _ -> "same as you"
            end,
        io:format("~s's total steps: ~p (~s)~n", [Name, Total, Comparison])
    end, friends_steps()).
```

* Sahad
* Sneha

1. Product Operations Analyst
1. Business Analyst


* [ ] sneha walked 10000 steps
* [x] sahad walked 10000 steps

| Name        | Mon     | Tue    |
| ------      | ---------   | ------ |
|Sahad | 7000 | 8000 |
|Sneha | 5000 | 7200 |

[My working space website](https://xylem.binalyto.com/app/home)

![Walk](https://www.citypng.com/photo/25085/hd-mickey-mouse-walking-cartoon-character-png)

> Walk Like Micheal Jackson

<!-- This is done by Me -->

___