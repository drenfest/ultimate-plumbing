<script>

</script>
<style>

</style>

<svelte:head>
	<title>Contact Aries Mechanical</title>
	<meta name="description" content="Customers rely on Aries Mechanic Inc. HVAC in Newark, IL to get the job done in a high-degree of professionalism and workmanship.">
</svelte:head>

<form action="" method="post">
	<div class="form-group">
		<h2>Your information</h2>
		<label for="name">Name
			<input class="form-control" id="name" type="text" name="name" />
		</label>
		<label for="email">Email
			<input class="form-control" id="email" type="email" name="email" />
		</label>
	</div>
	<div class="form-group">
		<h2>Service information</h2>
		<label for="type_of_unit">This Service is for:
			<select class="form-control" id="type_of_unit" name="type_of_unit">
				<option selected="selected" value="">Please select...</option>
				<option value="Furnace">Furnace</option>
				<option value="Air Conditioner">Air Conditioner</option>
				<option value="Hot Water Tank">Hot Water Tank</option>
				<option value="Other">Other</option>
			</select>
		</label>
		<label for="project_status">Project Status:
			<select class="form-control" id="project_status" name="project_status">
				<option selected="selected" value="">Please select...</option>
				<option value="Ready to Hire">Ready to Hire</option>
				<option value="Planning and Budgeting">Planning and Budgeting</option>
			</select>
		</label>
		<label for="how_did_you_hear_about_aries_">How Did You Hear About Us:
			<select class="form-control" id="how_did_you_hear_about_aries_" name="how_did_you_hear_about_aries_" value="">
				<option selected="selected" value="">Please select...</option>
				<option value="Direct Mail">Direct Mail</option>
				<option value="Internet Website">Internet Website</option>
				<option value="Newspaper">Newspaper</option>
				<option value="Previous Customer">Previous Customer</option>
				<option value="Referred by Others">Referred by Others</option>
				<option value="Sign on Building">Sign on Building</option>
				<option value="Sign on Service Truck">Sign on Service Truck</option>
				<option value="Social Media">Social Media</option>
				<option value="Television">Television</option>
				<option value="Yard Sign">Yard Sign</option>
				<option value="Yellow Page Book">Yellow Page Book</option>
				<option value="Other">Other</option>
			</select>
		</label>
	</div>
	<div class="form-group">
		<label for="brand_of_unit">Brand of Unit:
			<input class="form-control" name="brand_of_unit" type="text" value="">
		</label>
		<label for="age_of_unit">Age of Unit:
			<select class="form-control" id="age_of_unit" name="age_of_unit">
				<option selected="selected" value="">Please select...</option>
				<option value="1-5">1-5 years</option>
				<option value="6-10">6-10 years</option>
				<option value="11-15">11-15 years</option>
				<option value="16-24">16-24 years</option>
				<option value="25+">25 + years</option>
			</select>
		</label>
		<label for="last_time_unit_was_serviced">Unit Last Serviced:
			<select class="form-control" id="last_time_unit_was_serviced" name="last_time_unit_was_serviced">
				<option selected="selected" value="">Please select...</option>
				<option value="This Season">This Season</option>
				<option value="Less than 1 Year">Less than 1 Year</option>
				<option value="1-5 Years">1-5 Years</option>
				<option value="Over 5 Years">Over 5 Years</option>
				<option value="Never">Never</option>
			</select>
		</label>
		<label for="did_aries_install_your_system_">Did We Install Unit:
			<select class="form-control" id="did_aries_install_your_system_" name="did_aries_install_your_system_">
				<option selected="selected" value="">Please select...</option>
				<option value="Yes">Yes</option><option value="No">No</option>
				<option value="Unsure">Unsure</option>
			</select>
		</label>
	</div>
	<div class="form-group">
		<label for="nature_of_problem">Nature of Problem:
			<select class="form-control" id="nature_of_problem" name="nature_of_problem">
				<option selected="selected" value="">Please select...</option>
				<option value="Unit Not Running">Unit Not Running</option>
				<option value="No Hot Air">No Hot Air</option>
				<option value="No Cold Air">No Cold Air</option>
				<option value="A/C is Frozen">A/C is Frozen</option>
				<option value="Unit is Making a Strange Noise">Unit Making Strange Noise</option>
				<option value="No Heating to One Area of Home">No Heating to One Area of Home</option>
				<option value="Other">Other</option>
			</select>
		</label>
	</div>
	<div class="form-group">
		<label for="are_you_the_homeowner">Are You the Homeowner:
			<select class="form-control" id="are_you_the_homeowner" name="are_you_the_homeowner">
				<option selected="selected" value="">Please select...</option>
				<option value="Homeowner">Homeowner</option>
				<option value="Renter">Renter</option>
				<option value="Condo">Condo</option>
				<option value="Landlord">Landlord</option>
			</select>
		</label>
	</div>
	<div class="form-group">
		<label for="is_this_request_covered_by_insurance_">Request Covered by Insurance:
			<select class="form-control" id="is_this_request_covered_by_insurance_" name="is_this_request_covered_by_insurance_">
				<option selected="selected" value="">Please select...</option>
				<option value="Yes">Yes</option>
				<option value="No">No</option>
				<option value="Unsure">Unsure</option>
			</select>
		</label>
	</div>
	<p class="form-status" style="display:none;">Your Message Has Been Successfully Sent</p>
	<button class="btn btn-lg btn-primary">Submit Form</button>
</form>
