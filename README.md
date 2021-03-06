# Robot Simulator

## Background

### Step 1

The robot factory manufactures robots that have three possible movements:

* turn right
* turn left
* advance

Robots are placed on a hypothetical infinite grid, facing a particular
direction (north, east, south, or west) at a set of {x,y} coordinates, e.g.,
{3,8}.

### Step 2

The factory's test facility needs a program to verify robot movements.

There are a number of different rooms of varying sizes, measured in Robot
Units, the distance a robot moves when you instruct it to `advance`.

The floor of the room is a grid, each square of which measures 1 square RU
(Robot Unit).

The rooms are always oriented so that each wall faces east, south, west, and
north.

The test algorithm is to place a robot at a coordinate in the room, facing in
a particular direction.

The robot then receives a number of instructions, at which point the testing
facility verifies the robot's new position, and in which direction it is
pointing.

### Step 3

The robot factory's test facility has a simulator which can take a string of
letters and feed this into a robot as instructions.

- The letter-string "RAALAL" means:
  - Turn right
  - Advance twice
  - Turn left
  - Advance once
  - Turn left yet again
- Say a robot starts at {7, 3} facing north.
  Then running this stream of instructions should leave it
  at {9, 4} facing west.

## Tests
To run the specs follow these commands:
```shell
# first install the new gem to run the tests
gem sources -a http://flatiron:33west26@gems.flatironschool.com
gem install learn-co

# to run in the command line run
learn

#to run in the browser
learn -b
```
When you finish passing a test, remove the `x` from `xit` to convert it to a runnable test.

<a href='https://learn.co/lessons/robotSimulator.js' data-visibility='hidden'>View this lesson on Learn.co</a>
