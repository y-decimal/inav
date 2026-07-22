# Gliding related settings and configuration

## Introduction

As part of an overhaul of iNav's glide related functions, a few new settings and OSD elements have been added to iNav.
This document serves as an overview of these settings and elements, what they are and how to set/use them.

---
### CLI settings

- **osd_glide_sample_time_frame**
    - This setting controls the time frame over which OSD elements such as Glide Ratio (also sometimes referred to as glide slope), Glide Range and Glide Time are calculated. 
    - Think of it like over what time frame the values are averaged. If set very low, the values will represent the instantaneous conditions, as they are right now. If set very high, the values will represent the long term conditions, as they have been on average over the time frame

- **osd_glide_min_speed**
    - This setting sets the minimum speed you expect to be flying during glide and is important for the polar calculation. Usually this should be set at or slightly below the stall speed of your glider. 
    - Setting it too low can cause the polar calculation to display best sink speeds below what you're physically capable of flying. Setting it too high might cut off the actual lowest sink speed from your polar.

- **osd_glide_max_speed**
    - This setting sets the maximum speed you expect to be flying during glide and is important for the polar calculation. Usually this should be set at the maximum speed you intend to fly without a motor. If you don't know how fast you intend to glide beforehand, setting it to twice the minimum speed is usually a good starting point.
    - Setting this too low can cause the polar calculation to miss the actual best glide speed. Setting it too high will make the polar calculation inaccurate.

---

#### NOTE: the osd_glide_min_speed and osd_glide_max_speed *need* to be set correctly for polar calculation to work
