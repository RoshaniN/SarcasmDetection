# SarcasmDetection
Detection of sarcasm from news headlines using BERT



python3 ./run_glue.py --model_type bert --model_name_or_path bert-base-uncased --task_name sarcasm --do_train --do_eval --do_test --do_lower_case --data_dir data --max_seq_length 128 --per_gpu_eval_batch_size=8 --per_gpu_train_batch_size=8 --learning_rate 2e-5 --num_train_epochs 3.0 --output_dir /tmp/sarcasm/