Add the pipeline.config file here and make the necessary changes.

- num_classes: 26
- fine_tune_checkpoint: "training/TF2/pre-trained-models/faster_rcnn_resnet101_v1_1024x1024_coco17_tpu-8/checkpoint/ckpt-0"
- fine_tune_checkpoint_type: "detection"

For train_input_reader
- label_map_path: "data/label_map.pbtxt"
- input_path: "data/train.record"

For test_input_reader
- label_map_path: "data/label_map.pbtxt"
- input_path: "data/test.record"