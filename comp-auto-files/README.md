```
There are two files for each playback option.  Both files are created during
the recording process, however during playback only the xxxxxxxx.txt file is
used (the xxxxxxxx.speeds.txt file is only used for analysing the data in
the FileEditor and PathAnimator programs).

The files have names that follow the format: xxxxxxxx.txt and 
                                             xxxxxxxx.speeds.txt

See the file: filelist.txt for a list of the different auto mode playback
              files and what they try to do.


Details on the playback file formats are below:


The xxxxxxxx.txt file has 5 columns containing containing the following
info:   command   time   leftcmd   rightcmd   state
where:
        command is a two letter code indicating which subsystem the commands
                on that line are intended to drive.'
        time    is the time since the start of playback, commands will be
                run until the time read from the file exceeds the current
                time the playback session has been running. 
        leftcmd is the command for the left drive train, or the command for
                for a subsystem that only has a single input.
        rightcmd is the command for the right drive train, or zero if the
                 subsystem only has a single input
        state    is the command for subsystems which take a discrete input
                 such as a solenoid.

The two letter command codes for this robot are (see lib/Commands.java):
        "  " = None
         DT  = Drive Train
         EL  = Elevator
         CS  = Cube arm spinning wheels
         CA  = Cube arm open/close
         FB  = Four bar up/down
         XX  = End of file indication

Note, negative commands to the drive train cause the robot to move forward.

Note also that the end of the file for this robot will typically always
contain two lines, one to make sure the elevator motor is commanded to
stop, and one to indicate that the end of the playback file has been
reached, and typically look like:

EL   12.00655  0.00000  0.00000 1
XX 9999.00000 999.00000 999.00000 0


The xxxxxxxx.speeds.txt file has 9 columns containing the following
info: pass  time  dt  leftcmd  rightcmd  leftdist  rightdist  leftvel  rightvel
where:
      pass      is the pass through the robot code
      time      is the total time elapsed since recording started
      dt        is the delta time between the prior pass and this pass.
      leftcmd   is the command to the left drive train
      rightcmd  is the command to the right drive train
      leftdist  is the distance from the left drive train encoder
      rightdist is the distance from the right drive train encoder
      leftvel   is the velocity from the left drive train encoder
      rightvel  is the velocity from the right drive train encoder

Note also that the last line of this file should always contain
the line to indicate to various programs that real data has ended:
9999 9999.00000 9999.00000 999.00000 999.00000 9999.00000 9999.00000 999.00000 999.00000```
