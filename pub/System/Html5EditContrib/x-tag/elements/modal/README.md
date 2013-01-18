
## Syntax

The following code creates a modal that has a transparent overlay and will close when the ESC key is pressed.

```
<x-modal overlay esc-hide>
	<p>Hello Hello from this modal</p>
</x-modal>
```


## Events

```
	var modal = document.getElementsByNames('x-modal')[0];
	modal.addEventListener('modalhide', function(e){
		// this event is thrown when ESC is pressed.  If you don't want the modal to close
		// you can prevent it like so.
		e.preventDefault();
	});

```

## Usage

```

	var modal = document.createElement('x-modal');
	modal.innerHTML = "<p>Wow it's easy to use this modal.</p>";
	modal.setAttribute('overlay','');
	modal.setAttribute('esc-hide','');
	document.appendChild(modal);


```


