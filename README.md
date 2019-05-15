# Online_Image_Augmentor_tensorflow


# Online Image Augmentor in pure tensorflow  for image classification or image detection

:param image: HWC or CHW

:param input_shape: [h, w]

:param data_format: 'channels_first', 'channels_last'

:param output_shape: [h, w]

:param zoom_size: [h, w]

:param crop_method: 'random', 'center'

:param flip_prob: [flip_top_down_prob, flip_left_right_prob]

:param fill_mode: 'CONSTANT', 'NEAREST_NEIGHBOR', 'BILINEAR', 'BICUBIC'

:param keep_aspect_ratios: True, False

:param constant_values:

:param color_jitter_prob: prob of color_jitter

:param rotate: [prob, min_angle, max_angle]

:param ground_truth: [ymin, ymax, xmin, xmax, classid]

:param pad_truth_to: pad ground_truth to size [pad_truth_to, 5] with -1

:return image: output_shape

:return ground_truth: [pad_truth_to, 5] [ycenter, xcenter, h, w, class_id]



# Experimental Environment

python3.6 tensorflow1.12
    
