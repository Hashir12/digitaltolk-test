# digitaltolk-test
I have gone through the code, code was fine, some areas needed improvement, php standard recommendation standard was not followed, some changes i have made are the followoing

1) There were some conditions where `if` conditions could be easily converted into where clauses,
  `\DTApi\Repository\BookingRepository::sendNotificationTranslator`
2) Some cases i felt un-unnecessary data transformations were performed instead of using a single database query and un-unnecessary for loops and if statements were used, this is very important because this results in bad performance
`refactor/app/Repository/BookingRepository.php:414`
1) Code indentation
2) Removed unsed and un-unnecessary variables
3) Code formated according to php standard recommendation
4) Removed redundent if else statements
5) Removed `response()` method, laravel automatically converts data into appropriate response

I refactored `BookingController` completely, but i was unable to do the same for `BookingRepository`, please accept my apologies, please understand that i am doing a full time job including 2+ hours or commute,if i get selected for the job, i assure you i take my work very seriously.