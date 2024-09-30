This project demonstrates a bug issue with ABP Studio/ABP Suite Master / Child forms if a navigation property is used and there is more than one child form for the parent form.
The parent form in this case has a many-to-many Employees table which looks up employee records from the Employee table. Each Company can have Many Employees.
The many-to-many lookup works with Company without a problem, even after adding the Child Forms.
When ABP suite builds the navigation collection tab, an incorrect reference to the record id is created and the object is null.
This problem occurs when the Company form has more than one child form.

The second form breaks.

