$('div').on('inview', function(event, isInView) {
  if (isInView) {
    // element is now visible in the viewport
  } else {
    // element has gone out of viewport
  }
});
To stop listening for the event - simply unbind:

$('div').off('inview');
If you would like the event only to trigger once per element while the page is loaded, you can use the .one() method instead of .on():

$('div').one('inview', ...);



********
var $self = $(this);
$this.fromTo({from: 0, to: $this.data('value'), speed: 2500});
