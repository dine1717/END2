# Task 2



## Training Logs

    ======== Epoch 1 / 4 ========
    Training...
      Batch    40  of    241.    Elapsed: 0:00:13.
      Batch    80  of    241.    Elapsed: 0:00:27.
      Batch   120  of    241.    Elapsed: 0:00:40.
      Batch   160  of    241.    Elapsed: 0:00:54.
      Batch   200  of    241.    Elapsed: 0:01:08.
      Batch   240  of    241.    Elapsed: 0:01:22.

      Average training loss: 0.50
      Training epcoh took: 0:01:22

    Running Validation...
      Accuracy: 0.78
      Validation Loss: 0.48
      Validation took: 0:00:03

    ======== Epoch 2 / 4 ========
    Training...
      Batch    40  of    241.    Elapsed: 0:00:14.
      Batch    80  of    241.    Elapsed: 0:00:28.
      Batch   120  of    241.    Elapsed: 0:00:42.
      Batch   160  of    241.    Elapsed: 0:00:56.
      Batch   200  of    241.    Elapsed: 0:01:11.
      Batch   240  of    241.    Elapsed: 0:01:25.

      Average training loss: 0.30
      Training epcoh took: 0:01:26

    Running Validation...
      Accuracy: 0.81
      Validation Loss: 0.46
      Validation took: 0:00:03

    ======== Epoch 3 / 4 ========
    Training...
      Batch    40  of    241.    Elapsed: 0:00:15.
      Batch    80  of    241.    Elapsed: 0:00:29.
      Batch   120  of    241.    Elapsed: 0:00:44.
      Batch   160  of    241.    Elapsed: 0:00:58.
      Batch   200  of    241.    Elapsed: 0:01:13.
      Batch   240  of    241.    Elapsed: 0:01:28.

      Average training loss: 0.19
      Training epcoh took: 0:01:28

    Running Validation...
      Accuracy: 0.82
      Validation Loss: 0.50
      Validation took: 0:00:03

    ======== Epoch 4 / 4 ========
    Training...
      Batch    40  of    241.    Elapsed: 0:00:15.
      Batch    80  of    241.    Elapsed: 0:00:29.
      Batch   120  of    241.    Elapsed: 0:00:44.
      Batch   160  of    241.    Elapsed: 0:00:58.
      Batch   200  of    241.    Elapsed: 0:01:13.
      Batch   240  of    241.    Elapsed: 0:01:28.

      Average training loss: 0.13
      Training epcoh took: 0:01:28

    Running Validation...
      Accuracy: 0.83
      Validation Loss: 0.62
      Validation took: 0:00:03

    Training complete!
    Total training took 0:05:56 (h:mm:ss)
    Let's view the summary of the training process.



## Sample Outputs


    sentence  > jack hates sue and is loved by mary .
    predicted < acceptable
    true cls  = acceptable

    sentence  > everyone relies on someone . it ' s unclear who .
    predicted < acceptable
    true cls  = acceptable

    sentence  > the defendant denied the accusation .
    predicted < acceptable
    true cls  = acceptable

    sentence  > i ' m creating a committee . kim – you ' re in charge .
    predicted < acceptable
    true cls  = acceptable

    sentence  > vote for you !
    predicted < acceptable
    true cls  = unacceptable

    sentence  > i like bill ' s yellow shirt , but not max ' s .
    predicted < acceptable
    true cls  = acceptable

    sentence  > chocolate eggs were hidden from each other by the children .
    predicted < acceptable
    true cls  = unacceptable

    sentence  > the paper was written by john up .
    predicted < acceptable
    true cls  = unacceptable

    sentence  > the bucket was kicked by pat .
    predicted < acceptable
    true cls  = acceptable

    sentence  > i never know which papers sandy has read , but i usually know how many .
    predicted < acceptable
    true cls  = acceptable
