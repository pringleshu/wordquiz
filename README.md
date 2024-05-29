# wordquiz
having both English dictionary and quiz functions

## Motivation
I thought it would be nice to have a quiz function in the vocabulary to memorize English words quickly and for a long time.

## examples
Operation in the following way
int main ()
{
	
	printf(" *** Word Quiz *** \n\n") ;

	int cmd ;
	do {
		print_msdenu() ;

		cmd = get_command() ;
		switch (cmd) {
			case C_LIST : {
				list_wordbooks() ;
				break ;
			}

			case C_SHOW: {
				show_words() ;
				break ;
			}

			case C_TEST: {
				run_test() ;
				break ;
			}

			case C_EXIT: {
				return EXIT_SUCCESS ;
			}
		}
	}
	while (cmd != C_EXIT) ;


	return EXIT_SUCCESS ;
}

Has 4 menus

## Next steps:
A method of asking for hints will be added. 
The ability to add words will be added.
The ability to delete words will be added.
There will be an additional function that will show random questions.
