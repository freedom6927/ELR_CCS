# ELR_CCS
This is the Reproduce of method ELR_CCS

evaluation

CUDA_VISIBLE_DEVICES=0 python train_ELR_CCS_detected.py --id 'ELR_CCS' --batch_size 16 --model_method 'ELR_CCS' --evaluate True --model ./output/checkpoints/ELR_CCS/model_best.pth.tar


training
CUDA_VISIBLE_DEVICES=0 python train_ELR_CCS_detected.py --learning_rate 1e-4 --id 'ELR_CCS' --word_drop_out 0.2 --rnn_drop_out 0.2 --jemb_drop_out 0.2 --batch_size 32 --edge_gate_drop_out 0.0 --word_judge_drop 0.0 --model_method 'ELR_CCS' --max_epochs 30

