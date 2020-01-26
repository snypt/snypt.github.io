# Pushing your snypts

Now that you have created all the snypts you want you can push these snypts to a snypt board using the 
``snypt push`` command. Before running ``snypt push`` we should log into our snypt account. 
```cmd
snypt login
```
You will be promted to enter your Snypt account email and password. If you have not yet created account 
you can do so [here](https://www.snypt.io/signup);
```cmd
  ____                            _
 / ___|   _ __    _   _   _ __   | |_
 \___ \  | '_ \  | | | | | '_ \  | __|
  ___) | | | | | | |_| | | |_) | | |_
 |____/  |_| |_|  \__, | | .__/   \__|
                  |___/  |_|


? Enter your snypt e-mail address: youremail.com
? Enter your password: [input is hidden]

```

Once you are logged into your Snypt account run the following command to push your Snypts 
to the cloud

```cmd
snypt push
```
You will prompted to select a board to push your snypts to. If haven't let created a board you 
can create one directly from the command line. 

```cmd
? Please a board to push your data too:
  Board 3
  Board 2
  Board 1
> **create new board**
  forgot_last825
  Test board 123
  January Board
(Move up and down to reveal more choices)
```
After selecting a board you have the option to append to or overwrite the data in that board.
Selecting append will add the new snypts to the board keeping the existing content. Over write will 
erase existing content and add the new snypts.

```cmd
? How would you like to push this data?
> Append
  Overwrite data    
```

After selecting an option snypt will parse through your project, search for snypts, and save them
to the board you selected.
