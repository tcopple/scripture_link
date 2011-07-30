# Scripture Link

Start with:
    Recently I started reading the bible. I started with <span class="scripture">Isaiah 40:8;</span>
    then moved onto <span>Matthew 22:29</span> and finished with <span class="scripture">John 5:39; 16:13-15; 17:17;</span> 

Apply:

    $('.scripture').scriptureLink();

Finish with:
    Recently I started reading the bible.  I started with <a href="http://www.gnpcb.org/esv/search/?q=Isaiah+40:8;" target="_blank">Isaiah 40:8;</a>
    then moved onto <span>Matthew 22:29</span> and finished with <a href="http://www.gnpcb.org/esv/search/?q=John+5:39;+16:13-15;+17:17;" target="_blank">John 5:39; 16:13-15; 17:17;</a>

# Options 

  By default scriptureLink will send you to gnpcb.org with the esv version.  The link will also open in a new window.
  However you can change these defaults by passing options to scriptureLink:

    $('.scripture'.scriptureLink({
      link: function(text) { return "http://www.biblegateway.com/" + text; } //this function must return the value of the href attribute      
      new_target: true or false
    });

