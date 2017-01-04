# TripC-
school code for ProgOne

//MM
Pseudocode

# Firstly, print the total distance to be travelled for the trip 
cout << "We need to travel a distance of " << DISTANCE << " miles!" << endl;

#Ask for input from user and confirm
cout << "\nKindly enter the  miles per gallon your car gets ";
cin >> MilesPerGallon;
cout << "You have entered: " << MilesPerGallon <<" miles per gallon!" << endl;

# Then calculate the gallons of gas we would needfor the trip.
double gallonReq = DISTANCE / MilesPerGallon;
cout << "\nSo We would need " << setprecision(2) << fixed << showpoint << gallonReq << " gallons of gasoline for our trip." << endl;

#Ask the user for input and confirm
cout << "\nEnter the average speed at which the car travels per hour: ";
cin >> avgSpeedPerHr;
cout << "\nYou have entered that the car travels at an average speed of: " << avgSpeedPerHr << " miles per hour!" << endl;

#Then calculate the average speed at which we would be travelling
double reducedMileage = avgSpeedPerHr * 0.12; // 3% PER PERSON, TOTAL NUMBER OF PERSONS 4, TOGETHER 12%
double distPerGall = avgSpeedPerHr - reducedMileage;
cout << "but four of us travelling in our car would reduce the gas mileage by " << reducedMileage << endl;
cout << "miles per hour" << endl;
cout << "So we would be travelling at " << distPerGall << " miles per hour!" << endl;

#Ask the user for input again and Then calculate the number of days we would need to drive
cout << "\nHow many hours per day, would you wish to drive?: ";
cin >> HoursPerDay;
double hoursReq = DISTANCE / distPerGall;
double daysReq = ceil(hoursReq / HoursPerDay);
cout << "So you would require: " << setprecision(2) << fixed << showpoint << hoursReq << " hours to complete the trip " << endl;
cout << "or " << daysReq << " days!" << endl;

#Then Calculate total cost of gasoline
cout << "\nAs the cost of gasoline per gallon is $ " << setprecision(2) << fixed << showpoint << PRICEPERGALLON << endl;

double totcostGas = PRICEPERGALLON * gallonReq;
cout << "The total cost of gasoline for the trip would be $ " << setprecision(2) << fixed << showpoint << totcostGas << endl;	

# Calculate total cost of lodging	
cout << "\nThe cost of lodging per night is $ " << setprecision(2) << fixed << showpoint << LODGINGPERNIGHT << endl;
cout << "So the total cost of lodging for " << nightsReq << " nights would be $ " << setprecision(2) << fixed << showpoint << totCostLodge << endl;
	
# Calculate total cost of the trip
cout << "\nThe total cost for the trip would be " << setprecision(2) << fixed << showpoint << totCostTrip << endl;

