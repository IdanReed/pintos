 To add an alarm mega test changes were made to the following files:
 
    src/tests/threads/Make.tests 
        add alarm-mega to give path the src/tests/threads/alarm-mega.ck

    src/tests/threads/alarm-wait.c
        add test_alarm_mega function that interates 70 times
        
    src/tests/threads/tests.c
        add "alarm-mega" mapped to test_alarm_mega to allow for running the test with alarm-mega
        
    src/tests/threads/tests.h
        add extern dec for test_alarm_mega so that test.c can wait for def
        
    
Some other files were also changed (can be seen in commit history) to allow for running with QEMU.
