# Generate numbers in a certain range / Get True/False  according to a certain percentage


```python

$pip install generate-random-values-in-range
from generate_random_values_in_range import randomize_number,get_true_false_percent


for _ in range(200):
    randval = randomize_number(
        value=620,
        percent=20,
        percentage_substract_vs_add=70,
        minimum_to_allow=580,
        maximum_to_allow=700,
    )
    if _ % 20 == 0:
        print("")
    print(randval, end=" ")

694 666 643 580 614 619 700 700 580 653 700 580 583 603 646 700 580 609 580 580 
580 580 580 700 580 700 697 580 700 614 580 649 580 610 600 582 580 580 587 580 
605 580 580 595 602 620 584 592 700 700 698 580 580 609 580 622 644 580 580 580 
590 580 652 591 666 607 580 610 580 580 580 594 615 580 594 580 612 679 607 580 
639 700 621 665 587 622 585 580 599 580 580 600 580 580 700 700 580 580 599 580 
610 580 596 580 696 580 661 589 589 618 612 580 580 580 635 634 580 580 606 580 
581 580 612 580 580 580 602 580 580 700 580 580 580 580 700 580 580 580 691 609 
580 580 648 580 580 580 605 580 580 580 700 699 615 580 643 700 580 595 700 580 
697 580 580 630 580 580 585 582 580 593 619 580 596 688 580 581 700 580 580 580 
627 580 580 580 584 598 580 610 580 583 590 700 580 675 580 684 580 590 580 700 


for _ in range(100):
    randval = get_true_false_percent(percent_true=80)
    if _ % 20 == 0:
        print("")
    if randval is True:
        print(randval, end="  ")
    else:
        print(randval, end=" ")

True  False True  True  True  False True  True  True  True  True  True  True  True  True  True  True  True  True  True  
True  True  False True  True  False True  True  True  True  True  True  True  True  True  True  True  True  True  True  
True  True  True  True  True  False True  True  False True  True  True  True  True  True  True  True  False True  True  
False True  True  True  True  True  True  False False True  True  True  True  True  True  True  True  True  True  False 
True  True  False True  True  True  True  True  True  True  True  True  True  False True  True  True  False True  True  		

```