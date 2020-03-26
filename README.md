# SarcasmDetection
Detection of sarcasm from news headlines using BERT



python3 run_glue.py --model_type bert --model_name_or_path bert-base-uncased --task_name sarcasm --do_train --do_eval --do_test --do_lower_case --data_dir data --max_seq_length 32 --per_gpu_eval_batch_size 32 --per_gpu_train_batch_size 32 --per_gpu_test_batch_size 32 --learning_rate 2e-5 --num_train_epochs 3.0 --output_dir output

#for testing only
python3 run_glue.py --model_type bert --model_name_or_path bert-base-uncased --task_name sarcasm --do_test --do_lower_case --data_dir data --max_seq_length 32 --per_gpu_eval_batch_size 32 --per_gpu_train_batch_size 32 --per_gpu_test_batch_size 32 --learning_rate 2e-5 --num_train_epochs 3.0 --output_dir output

#for training and eval
python3 run_glue.py --model_type bert --model_name_or_path bert-base-uncased --task_name sarcasm --do_train --do_eval --do_lower_case --data_dir data --max_seq_length 32 --per_gpu_eval_batch_size 32 --per_gpu_train_batch_size 32 --per_gpu_test_batch_size 32 --learning_rate 2e-5 --num_train_epochs 3.0 --output_dir output