These files are the files currently on the RoboRIO on the competiton bot at the
end of hartford with the tweaks made over the competition.

These files are not consistent between the xxxxxx.txt and xxxxxx.speeds.txt

These files don't have the shortened left2scale_short.txt file made in the
championship match that was copied over the other left2scale files so that
we wouldn't interfere with 195 crossing over if the scale was on the left.

Differences from what we started the hartford competition with:

center2left.speeds.txt              -- no change
center2left.txt                     -- from 5.66 to 6.02 left and right power set to zero (better shot a picking up 2nd cube)
                                    -- from 10.00 to 10.85 right power copied to left power (try not to align to switch better)


center2right.speeds.txt             -- no change
center2right.txt                    -- from 0.0 to 0.56 left and right power set to zero (try to keep bot from going too far right)
                                    -- from 7.2 to 7.78 left and right power set to zero (try to keep bot from going too far right on 2nd cube)

center2right_simple.speeds.txt      -- no change  note, only used if NGD (No Game Data)
center2right_simple.txt             -- no change

left2scale.speeds.txt               -- no change
left2scale.txt                      -- at 2.4 command cube spinners to hold on to cube
                                    -- from 4.0 to 4.44 set elevator power to near zero to no hit upper limit so hard
                                    -- at 5.34 set cube spinners to zero when dropping cube on scale

left2scale_2cube.speeds.txt         -- no change, same as left2scale.speeds.txt 
left2scale_2cube.txt                -- same changes as left2scale.txt above

left2scale_noswitch.speeds.txt      -- no change, same as left2scale.speeds.txt
left2scale_noswitch.txt             -- same changes as left2scale.txt above

left2scale_short.speeds.txt         -- no change
left2scale_short.txt                -- from 1.26 to 2.0 data removed (file ends at 1.26 now to keep from going into null zone)

left2scale_short_switch.speeds.txt  -- no change
left2scale_short_switch.txt         -- no change

left2scaleright.speeds.txt          -- no change
left2scaleright.txt                 -- from 1.32 to 2.2 left and right power increase by 0.1 (go a little farther, and not hit cubes behind switch when crossing over)

right2scale.speeds.txt              -- no change
right2scale.txt                     -- from 1 to 1.7 copy right power to left power (keep bot from heading under scale)
                                    -- from 4.5 to 5.0 seconds add left right backup power at 0.2 (to back out from under scale)
                                    -- original lines from 4.5 to end have time shifted up by 1 second
									
right2scale_2cube.speeds.txt        -- no change
right2scale_2cube.txt               -- same changes as right2scale.txt above

right2scale_noswitch.speeds.txt     -- no change
right2scale_noswitch.txt            -- same changes as right2scale.txt above

right2scale_short.speeds.txt        -- no change
right2scale_short.txt               -- from 1.26 to 2.0 data removed (file ends at 1.26 now to keep from going into null zone)

right2scale_short_switch.speeds.txt -- no change
right2scale_short_switch.txt        -- no change

right2scaleleft.speeds.txt          -- no change
right2scaleleft.txt                 -- no change
