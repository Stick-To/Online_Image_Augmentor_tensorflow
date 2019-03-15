# Online_Image_Augmentor_tensorflow


#Online Image Augmentor in pure tensorflow  for image classification or image detection



"""

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
    
    :param rotate_range:
    
    :param ground_truth: [ymin, ymax, xmin, xmax, classid]  if None, just return image
    
    :param pad_truth_to: pad ground_truth to size [pad_truth_to, 5] with -1; must grater that num of bbox;
    
    :return image: output_shape, HWC or CHW corresponding to input image
    
    :return ground_truth: [pad_truth_to, 5]
    
"""
    
    
image_augmentor_config = {

    'data_format': 'channels_last', 
    
    'output_shape': [300, 300],  
    
    'zoom_size': [320, 320],
    
    'crop_method': 'random',
    
    'flip_prob': [0., 0.5],
    
    'fill_mode': 'BILINEAR',
    
    'keep_aspect_ratios': True,
    
    'constant_values': 0.,
    
    'rotate_range': [-5., 5.],
    
    'pad_truth_to': 60,
    
}
