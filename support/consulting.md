---
title: "Consulting Resources"
---

# Consulting Resources

Bugzilla is made available free of charge, without warranty. Support
provided for free by Bugzilla team members via email or newsgroups also
comes without warranty. If you need higher-level support, the following
contractors and businesses (some of whom may be members of the Bugzilla
team) may be able to help you.

Bugzilla consultants could help you save time installing and
administering your Bugzilla system. They could also let you know the
best way to make changes to your installation.

This page lists contractors and businesses who have declared themselves
available for Bugzilla consulting work. There is no screening process as
a prerequisite to being on this list, and as such, no guarantee is
supplied as to the quality of their work. If you wish to hire them, you
will need to assess this for yourself. Listings are in random order and
will display in a different order every time the page is loaded in order
to be fair to everyone. Companies or individuals who are current
contributors to the Bugzilla Project are sorted to the top of the list
and have (contributor) next to their name.

All information (including comments) appears as given by the person
requesting the listing (excepting editorial changes to make it fit the
format of this web page).

If you wish to be added to this list, or if you discover someone on this
list who is no longer in business or no longer offering Bugzilla
support, please email <justdave@bugzilla.org> with the relevant
information.

<script src="https://yui-s.yahooapis.com/2.9.0/build/yahoo/yahoo-min.js"></script>
<script src="https://yui-s.yahooapis.com/2.9.0/build/dom/dom-min.js"></script>
<script type="text/javascript">
  function updateList(regionSelect) {
      var region = regionSelect.value;
      var vendor_list = document.getElementById('vendor_list');
      var all_lis = vendor_list.getElementsByTagName('li');
      if (region) {
          for(var i = 0; i < all_lis.length; i++) {
              YAHOO.util.Dom.setStyle(all_lis[i], 'display', 'none');
          }
          var show_lis =
            YAHOO.util.Dom.getElementsByClassName(region, 'li', vendor_list);
          for (var i = 0; i < show_lis.length; i++) {
              YAHOO.util.Dom.setStyle(show_lis[i], 'display', '');
          }
      }
      else {
         for(var i = 0; i < all_lis.length; i++) {
              YAHOO.util.Dom.setStyle(all_lis[i], 'display', '');
          }
      }
  }
</script>

<form method="GET" action="#">
  <div><b>Region:</b>
   <select class="custom-select" name="region" id="region" onchange="updateList(this)">
     <option value="">All</option>
   </select>
  </div>
</form>

<ul id="vendor_list"></ul>
<noscript>Sorry, this page requres JavaScript!</noscript>

<script src="https://lists.bugzilla.org/cgi-bin/bz_vendors.cgi?refresh=1"></script>
<script type="text/javascript">
  var regionSelect = document.getElementById('region');
  for(var i = 0; i < regions.length; i++) {
      var opt = new Option(regions[i]);
      regionSelect.options[i + 1] = opt;
  }
  var vendor_list = document.getElementById('vendor_list');
  vendor_list.innerHTML = vendors;
</script>
