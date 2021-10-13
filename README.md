![](https://komarev.com/ghpvc/?username=talktovik&style=flat-square)



I am trying to write clean, optimised and meaningful code.
Simple just like that.

I know, Whatever.

For more Info do please check the website mentioned in bio.

(dir -include *.cpp, *.h -recurse | select-string "^(\s*)//" -notMatch | select-string "^(\s*)$" -notMatch).Count


2 lines (20 sloc)  530 Bytes
   
name: "📅 Isometric commit calendar"
cost: 1-2 GraphQL requests + 1 GraphQL request per year
category: github
index: 0
supports:
  - user
inputs:

  # Enable or disable plugin
  plugin_isocalendar:
    description: Display an isometric view of your commits calendar
    type: boolean
    default: no

  # Set time window shown by isometric calendar
  plugin_isocalendar_duration:
    description: Set time window shown by isometric calendar
    type: string
    default: half-year
    values:
      - half-year
      - full-year
