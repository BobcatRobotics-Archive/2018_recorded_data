These files are the files currently on the RoboRIO on the competiton bot at the
end of hartford with the tweaks made over the competition.

These files are not consistent between the xxxxxx.txt and xxxxxx.speeds.txt

These files don't have the shortened left2scale_short.txt file made in the
championship match that was copied over the other left2scale files so that
we wouldn't interfere with 195 crossing over if the scale was on the left.

Differences from the hartford_auto_files_raw directory:

center2left.speeds.txt              -- no change
center2left.txt                     -- no change

center2right.speeds.txt             -- no change
center2right.txt                    -- no change

center2right_simple.speeds.txt      -- no change
center2right_simple.txt             -- no change

left2scale.speeds.txt               -- no change
left2scale.txt                      -- no change

left2scale_2cube.speeds.txt         -- no change
left2scale_2cube.txt                -- no change

left2scale_noswitch.speeds.txt      -- no change
left2scale_noswitch.txt             -- no change

left2scale_short.speeds.txt         -- no change
left2scale_short.txt                -- from 1.0 to 1.26 removed (file ends at 1.0 now to keep blocking 195 type team)
                                    -- NOTE:this change made on bot in Hartford champs and copied to:
                                    --      left2scale.txt, left2scale_noswitch.txt & left2scale_2cube.txt
                                    --   *** the above files need to be restored on RoboRIO before NE champs ***

left2scale_short_switch.speeds.txt  -- no change
left2scale_short_switch.txt         -- Removed 0.0 to 0.3 lines are updated time, as power wasnt changing and velocity was 0
                                    -- Removed 1.28 through 1.42 seconds to try and shorten travel by approx. 12 inches.

left2scaleright.speeds.txt          -- no change
left2scaleright.txt                 -- no change

right2scale.speeds.txt              -- no change
right2scale.txt                     -- no change
									
right2scale_2cube.speeds.txt        -- no change
right2scale_2cube.txt               -- no change

right2scale_noswitch.speeds.txt     -- no change
right2scale_noswitch.txt            -- no change

right2scale_short.speeds.txt        -- no change
right2scale_short.txt               -- from 1.0 to 1.26 data removed (file ends at 1.0 now to keep blocking 195 type team)

right2scale_short_switch.speeds.txt -- no change
right2scale_short_switch.txt        -- no change

right2scaleleft.speeds.txt          -- no change
right2scaleleft.txt                 -- no change
