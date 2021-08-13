# PI-Net
CVPR 2021 PI-Net Code

1. train_Auto_Encoder_G_mapping_noC.py
    -> main()
    -> train         = EasyDict(run_func_name='training.training_loop_Auto_Encoder_G_mapping_noC.training_loop')
    -> D_loss        = EasyDict(func_name='training.loss_Auto_Encoder_G_mapping_noC.D_loss')
    -> M_loss        = EasyDict(func_name='training.loss_Auto_Encoder_G_mapping_noC.Mapping_loss', feature_scale=0.00005, D_scale=0.1)
    -> M_lossKl      = EasyDict(func_name='training.loss_Auto_Encoder_G_mapping_noC.Mapping_loss_kl', feature_scale=0.00005, D_scale=0.1)
    -> reM_loss      = EasyDict(func_name='training.loss_Auto_Encoder_G_mapping_noC.reMapping_loss', feature_scale=0.00005, D_scale=0.1)
    -> D_loss        = EasyDict(func_name='training.loss_Auto_Encoder_G_mapping_noC.D_loss')

2. (a) training_loop_Auto_Encoder_G_mapping_noC and (b) loss_Auto_Encoder_G_mapping_noC are both .py files that have been placed in the folder. 

3. That is, training_loop is the function in training_loop_Auto_Encoder_G_mapping_noC.py, which is the main training process.  The loss function used is in loss_Auto_Encoder_G_mapping_noC.py.

4. The process of adding differential privacy noise is in PI-Net--4.ipynb.
