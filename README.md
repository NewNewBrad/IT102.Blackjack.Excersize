# IT102.Blackjack.Excersize

Your job: improve this code by adding some sort of iteration for flow control. The player should not be limited to 3 cards - the player should be able to take hits as long as she desires. You don't have to take this simulation all the way to a real Blackjack game. That may come later. But for now, just add the iteration feature. Note: for more on the random number generation used in this example, please refer to this discussion.

----------------------------------

<!DOCTYPE html>
<html>
<body>

<h1>Blackjack</h1>

<script>
//initialize all variables
var card = 0;
var total = 0;
var hitMe = true;
var dealer = 0;

//1st card
hitMe = prompt("Current total: " + total, "Take a card? Y/N");
if (hitMe == "Y"){hitMe = true;}
else {hitMe = false;}
if(hitMe){
card = Math.ceil(11*Math.random());
total += card;
}

//2nd card
hitMe = prompt("Current total: " + total, "Take a card? Y/N");
if (hitMe == "Y"){hitMe = true;}
else {hitMe = false;}
if(hitMe){
card = Math.ceil(11*Math.random());
total += card;
}

//3rd card
hitMe = prompt("Current total: " + total, "Take a card? Y/N");
if (hitMe == "Y"){hitMe = true;}
else {hitMe = false;}
if(hitMe){
card = Math.ceil(11*Math.random());
total += card;
}

//final total
dealer = Math.ceil(11*Math.random()) + Math.ceil(11*Math.random()); //dealer always takes 2 cards
alert("Your hand is worth " + total + ". Dealer got " + dealer + ".");

</script>

</body>
</html>
