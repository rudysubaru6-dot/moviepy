

   from moviepy.editor import VideoFileClip

# Load your video
clip = VideoFileClip("zerotwo.mp4")

# Reverse it
reversed_clip = clip.fx(lambda c: c.fx(vfx.time_mirror))

# Save output
reversed_clip.write_videofile("zerotwo_reversed.mp4", codec="libx264")
