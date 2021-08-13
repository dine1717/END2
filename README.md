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


# Task 3

## Training Log

![Screenshot 2021-08-14 at 12 17 34 AM](https://user-images.githubusercontent.com/73247157/129405262-34f6dae8-b745-400c-91ca-e3548fc316c5.png)


# Output Logs:

    Text  > Why don't people look things up on the internet before asking Quora?
    Pred  < Why do so many people ask questions on Quora?
    Truth = Why don't Quora people just look up the answer on Google?

    Text  > What is an example of moral conflict?
    Pred  < What is a good example of moral conflict?
    Truth = What is a moral conflict? What are examples of this?

    Text  > Are the orbits of the planets synchronized on the same plane?
    Pred  < Paraphrase: Are the orbits of the planets synchronized on the same plane?
    Truth = Are the orbits of each planets coplanar?

    Text  > For what reasons have you been edit blocked on Quora?
    Pred  < What do you think is the reason you have been blocked on Quora?
    Truth = If you've never been edit blocked on Quora, to what do you attribute that?

    Text  > I do masturbation twice in a day. Does masturbation affects men's sperm count or does it cause infertility?
    Pred  < Paraphrase: I do masturbation twice a day. Does masturbation affect men's sperm count or does it cause infertility?
    Truth = Does masturbation cause infertility?

    Text  > What would happen if I went back in time and killed hitler as a baby?
    Pred  < What would happen if I went back in time and killed hitler as a baby?
    Truth = If I had a time machine, what would happen if I went back in time to assassinate Hitler?

    Text  > How many bones are in a shark's body?
    Pred  < How many bones are in a shark's body?
    Truth = How many bones do sharks have?

    Text  > Is it safe to lose 75 pound in 2 months?
    Pred  < Par it safe to lose 75 pounds in 2 months?
    Truth = What are some ideas on how to lose 75 pounds in 2 months?

    Text  > Should we buy unboxed phones?
    Pred  < Is should I buy unboxed phones?
    Truth = Should we buy unboxed mobiles?

    Text  > English cooking dominated early national cooking ; but as new immigrants arrived from other countries, other colonial soups gained popularity.
    Pred  < Paraphrase: English cooking dominated early national cooking ; but as new immigrants arrived from other countries, other colonial soups gained popularity.
    Truth = Cooking dominated early national cuisine, but as new immigrants arrived from other countries, other colonial soups gained popularity.

    Text  > If you want to guess the average IQ of people on Quora, what would it be?
    Pred  < Paraphrase: If you want to guess the average IQ of people on Quora, what would it be?
    Truth = What is the average IQ on Quora?

    Text  > Have you ever seen any ghost?
    Pred  < What you have ever seen a ghost?
    Truth = Has anyone ever seen real ghosts/scientifically unexplainable things?

    Text  > How can I overcome lack of motivation?
    Pred  < How do I overcome lack of motivation?
    Truth = How does one overcome extreme laziness and lack of motivation?

    Text  > How exactly does banning Rs 500 and Rs 1000 notes curb the problem of black money?
    Pred  < How will banning 500 and 1000 rupee notes help in curbing black money?
    Truth = How banning 500 and 1000 rs note will help fight corruption in India?

    Text  > What was the craziest thing you have done?
    Pred  < What is the craziest thing you have ever done?
    Truth = What is the craziest thing you have ever done in your lifetime?

    Text  > How could I get rid of Facebook addiction?
    Pred  < How do I get rid of Facebook addiction?
    Truth = What should I do to get rid of addictions?
