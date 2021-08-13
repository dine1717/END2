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

    Text  > The medals were presented by Carlo Croce , IOC member , New Zealand and Barbara Kendall , President of World Sailing .
    Pred  < Paraphrase : The medals were presented by Carlo Croce, IOC member, New Zealand and Barbara Kendall, President of World Sailing.
    Truth = The medals have been presented by Carlo Croce , IOC - member , New Zealand , and Barbara Kendall , president of World Sailing .

    Text  > The BBC College of Journalism was opened as an e-learning course series in June 2005 , with Vin Ray as Executive Editor . Its first Director was Kevin Marsh .
    Pred  < Paraphrase : The BBC College of Journalism was opened in June 2005 as an e-learning course series with Vin Ray as Executive Editor, and its first director was Kevin Marsh.
    Truth = In June 2005 , the BBC College of Journalism was opened as an e-learning series with Vin Ray as Executive Editor , whose first director was Kevin Marsh .

    Text  > The original team was produced by the writer Sal Buscema and artist Roy Thomas in `` The Avengers '' # 71 ( December 1969 ) .
    Pred  < Paraphrase : The original team was produced by writer Sal Buscema and artist Roy Thomas in `` The Avengers '' # 71 ( December 1969 ).
    Truth = The original team was created by writer Sal Buscema and artist Roy Thomas in `` The Avengers '' # 71 ( December 1969 ) .

    Text  > Katuwana Divisional Secretariat is a Divisional Secretariat of Southern Province , of Hambantota District , Sri Lanka .
    Pred  < Paraphrase : Katuwana Divisional Secretariat is a divisional secretariat of the Southern Province, of Hambantota District, Sri Lanka.
    Truth = Katuwana Divisional Secretariat is a Divisional Secretariat of the Southern Province of Hambantota District , Sri Lanka .

    Text  > Mats Wilander defeats Anders Järryd , 6 -- 4 , 3 -- 6 , 7 -- 5 .
    Pred  < Paraphrase : Mats Wilander defeats Anders Järryd, 6 -- 4, 3 -- 6, 7 -- 5.
    Truth = Mats Wilander defeats Anders Järryd , 6 -- 4 , 3 - 6 , 7 -- 5 .

    Text  > The Communists firmly believed that the Central Intelligence Agency supported these protests discreetly financially and otherwise .
    Pred  < Paraphrase : The Communists firmly believed that the Central Intelligence Agency quietly supported these protests financially and otherwise.
    Truth = The communists strongly believed that the Central Intelligence Agency discreetly supported these protests , financially and otherwise .

    Text  > Another way to control the population of deer is to regulate the birth rate .
    Pred  < Paraphrase : Another way to control the population of deer is to regulate the birth rate.
    Truth = Another way to regulate deer population is to control the birth rate .

    Text  > In his Berlin study , three figures hanged on the wall : Schopenhauer , Maxwell , Faraday .
    Pred  < Paraphrase : In his Berlin study, three figures were hanged on the wall : Schopenhauer, Maxwell, Faraday.
    Truth = In his Berlin study , three figures hang on the wall : Faraday , Maxwell , Schopenhauer .

    Text  > The port of Tubarão is a port at Espírito Santo , near the city of Vitória in Brazil .
    Pred  < The port of Tubarão is a port at Espírito Santo, near the city of Vitória in Brazil.
    Truth = The Port of Tubarão is a port in Espírito Santo , near the city of Vitória in Brazil .

    Text  > Tell his father , Zac MacGuire ( Charlie Clausen ) and Evie immediately .
    Pred  < Paraphrase : Tell his father, Zac MacGuire ( Charlie Clausen ) and Evie immediately.
    Truth = Tell him immediately his father , Charlie Clausen ( Zac MacGuire ) and Evie .

    Text  > He was born in Frederiksberg and has died in Copenhagen .
    Pred  < He was born in Frederiksberg and died in Copenhagen.
    Truth = He was born in Frederiksberg and died in Copenhagen .

    Text  > When the PPC is temporarily disrupted , especially the PPC of the right hemisphere , memory across saccades is significantly weakened .
    Pred  < Paraphrase : When the PPC is temporarily disrupted, especially the Ppc of the right hemisphere, memory across saccades is significantly weakened.
    Truth = When the PPC is temporarily disrupted , especially the PPC on the right , memory of saccades is significantly weakened .

