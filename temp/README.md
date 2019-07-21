# 训练

小样本

```bash
python style.py --checkpoint-dir temp/checkpoint --style temp/5_seconds_1.jpg --train-path temp/train --epochs 100 --batch-size 2 --checkpoint-iterations 20
```

```bash
python style.py --checkpoint-dir temp/checkpoint --style temp/5_seconds_1.jpg --train-path temp/train --vgg-path "D:/data/imagenet-vgg-verydeep-19.mat" --batch-size 2 --checkpoint-iterations 500
```



```bash
python style.py --checkpoint-dir temp/checkpoint --style temp/5_seconds_1.jpg --train-path temp/train --batch-size 2 --checkpoint-iterations 500
```

coco2014

```bash
python style.py --checkpoint-dir temp/checkpoint --style temp/5_seconds_1.jpg --train-path data/train2014 --epochs 1 --batch-size 2 --checkpoint-iterations 500
```

```bash
python style.py --checkpoint-dir temp/checkpoint --style temp/5_seconds_1.jpg --train-path "D:/data/VOC2012/JPEGImages" --vgg-path "D:/data/imagenet-vgg-verydeep-19.mat" --epochs 1 --batch-size 2 --checkpoint-iterations 500
```

VOC2012

```bash
python style.py --checkpoint-dir temp/checkpoint --style temp/5_seconds_1.jpg --train-path data/VOC2012/JPEGImages --epochs 1 --batch-size 2 --checkpoint-iterations 500
```

```bash
python style.py --checkpoint-dir temp/checkpoint --style temp/5_seconds_1.jpg --train-path "D:/data/VOC2012/JPEGImages" --vgg-path "D:/data/imagenet-vgg-verydeep-19.mat" --epochs 1 --batch-size 2 --checkpoint-iterations 500
```




# 预测

```bash
python evaluate.py --checkpoint temp/checkpoint --in-path temp/input --out-path temp/result --allow-different-dimensions
```

```bash
python transform_video.py --checkpoint temp/checkpoint --in-path temp/input/fox.mp4 --out-path temp/result/fox.mp4
```

