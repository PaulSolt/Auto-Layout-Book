# Auto Layout Book
Paul Solt
<Paul@SuperEasyApps.com>
9-18-2018

**Topic:** iPhone App UI Design with Auto Layout and Storyboards

My rough draft outline for the [Auto Layout Book](http://bit.ly/AutoLayoutBook). Chapters and ideas are subject to change.

NOTE:  You can send me an [email](Paul@SuperEasyApps.com) if you want something included.

## Chapter 1: Auto Layout 101 

1. Why
	2. Examples of iPhone Sizes (Screenshots of an app)
	3. Accessibility (larger fonts)
	4. Responsive designs
	5. Rules for positions/sizes
	6. Size + position
		1. Coordinate system demo (download app)
	 	2. Points vs. pixels
		3. Vector vs. pixels
			4. 1x, 2x, 3x
			5. PDF vectors
			6. Preserving vector data (scaling up for accessibility)
9. Constraints explained
	10. Anotomy
	11. Constant
	12. Relation
	13. Multiplier
	14. Priority 
	14. Multiple constraints
8. Dive in: Real World Example
	9. Add constraints to the Tip Calculator app
		10. Centering Content in Container Views
		11. Equal width contraints
		12. Structural vs. accessory views
	13. Images
		14. Content mode
		15. Clipping
		16. Stretching
	18. Undo/redo
	19. Saving copies vs. Version Control (Github)
	18. Challenge
		19. Add iPhone X support (Safe Areas)
21. How
	3. 7 Ways to add constraints
2. Colors of Auto Layout
3. Breaking Constraints (unpredictable behavior)
	4. Common Errors
	5. Let's break it
4. Size Classes + Rotation
	5. We won't be using in this beginner's book
	6. Many popular apps don't support rotation (Simplify)
	7. iPad vs. iPhone
	8. iPad Splitview
9. The Obsolete iPhone SE (Design considerations)
7. Design + 
9. Welcome to Xcode
	10. Panels
	11. Issue Navigator
	12. Document Outline
	13. Storyboard Canvas
	14. Auto Layout's Hidden Error Panel
15. Images + Asset Catalog
	16. Slicing
	17. Stretchable images
	18. Template images

4. Rules for different screen types
5. How to add constraints (Ways to add constraints: 1100 words)
6. Real world example (build an app)
	1. Tip Calculator (layout)
	2. Challenge: do it again from scratch
		1. Watch how I layout for iPhone 8
	3. Add iPhone X support (Safe Areas)
	4. Add iPhone 8 Plus support (larger … button stretching)
	5. Add iPhone SE support (smaller buttons 44pt)
	6. iPad + Split view (separate chapter)
7. Let's break it (Fail early, try, fail, retry)
	1. clue as to why things aren't working as planned
	2. iOS examples (mac separate book)
8. 3 page pamphlet (2 minute video as to why/how)
9. Working code for 1st two chapters (easy to follow)
	5. Keep them interested
10. Practical tutorials

## Chapter 2: Auto Layout Fundamentals

1. Layout for one device
	2. Keep it simple, get something working
	3. Design for iPhone 8 (or iPhone X)
	4. Add constraints 
	5. Tweak for other screen sizes (Repeat)
6. Types of layout
	7. Percentage-based layouts
	8. Fixed layouts
	9. Relative layouts
10. Building blocks
	11. Structure views
	12. Accessory views
13. Constraint 101
	14. Anatomy of a constraint
15. Single screen vs. scrollable screen
	16. Different design considerations with layout
	17. Scrollable interface for super large fonts (edge case and more work)
18. Intrinsic Content Size (other section?)
	19. Brief overview
20. Data driven UI vs. static content
21. Margins
22. Safe areas
23. Localization
24. Button sizes
	25. Apple’s iOS HIG
	26. Apple’s macOS HIG
27. Accessibility
	28. Dynamic Type
	29. Voice over
		30. UI testing
31. Preview
	32. Device > Simulator > Preview
	33. Test it
	34. Edge cases (sample data)
	35. UITests 
	36. Dark mode
37. Rotation
	38. Many apps do not support rotation (Facebook or Instagram)
		39. Unless it’s video content



## 30-Day Auto Layout Challenge


1. 30DaysAutoLayout
2. Pinterest Mood board
3. Find what you like, mimic it

## Troubleshooting Auto Layout

1. When things don’t work like you expect
2. Fixing 9 common beginner mistakes  
3. Bad advice: When to ignore Xcode errors and warnings
4. Daily Log (Markdown)
