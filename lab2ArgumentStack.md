"threads/init.c:: main>run_actions (argv)>run_task > process_execute(process.c)" is called
"userprog/process.c:: process_execute() > thread_create > start_process > load > setup_stack"

uk@uk-com:~/os/pintos/src/userprog/build$ pintos-mkdisk fs.dsk --filesys-size=2
uk@uk-com:~/os/pintos/src/userprog/build$ pintos -q -f
uk@uk-com:~/os/pintos/src/userprog/build$ pintos -p ../../examples/echo -a echo -- -q
pintos -q run "echo My stack_setup() works"
