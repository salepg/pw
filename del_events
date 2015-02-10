//deletes events that older than today
	foreach($page->events as $e) {
		// get date
		$ed = $e->date;
		//check against today
		if(time() > $ed) {
			$page->of(false);
                        //remove is the right way from wirearray
			$page->events->remove($e);
			$page->save();
		}
	}
