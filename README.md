# phemplate
phemplate



//---------------------------------------------------------------------------//
// author: pukomuko <salna@ktl.mii.lt> 
// date:   2001.03.15
// web:    http://pukomuko.esu.lt
// info:   template engine
//
//
//---------------------------------------------------------------------------//
// copyleft license
//
// this software is provided 'as-is', without any express or implied
// warranty. in no event will the authors be held liable for any damages
// arising from the use of this software.
//
// permission is granted to anyone to use this software for any purpose,
// including commercial applications, and to alter it and redistribute it
// freely, subject to the following restrictions: 
//
// 1. the origin of this software must not be misrepresented;
//	  you must not claim that you wrote the original software. 
//	  if you use this software in a product, an acknowledgment 
//	  in the product documentation would be appreciated but is not required.
//
// 2. altered source versions must be plainly marked as such, 
//	  and must not be misrepresented as being the original software.
//
// 3. mail about the fact of using this class in production 
//	  would be very appreciated.
//
// 4. this notice may not be removed or altered from any source distribution.
//
//---------------------------------------------------------------------------//
// changes:
//
//	2004.04.21
//		- warining on empty file
//		* v1.10.1
//
//	2004.03.04
//		+ TPL_LOOPOPT -> TPL_OPTLOOP
//		+ TPL_PARSEDLOOP -> TPL_PARSEDLOOP
//		* v1.10
//
//	2004.03.03
//		+ TPL_LOOP_INNER_PARSED
//		+ TPL_LOOP_INNER_OPTIONAL
//		* v1.10beta2
//
//	2004.03.02
//		+ TPL_STRIP_UTF_HEADER
//		+ TPL_PARSEDLOOP
//		+ TPL_LOOPOPT
//		* v1.10beta
//		+ utf header matching
//
//	2004.03.01
//		- process() bugfix
//		* v1.9.4
//
//	2003.10.20
//		- parse() bugfix
//		* v1.9.3
//
//	2003.08.12
//		- remove_nonjs bugfix
//		* v1.9.2
//
//	2003.06.29
//		* optional now works with 0 and '0'
//		* v1.9.1
//
//	2003.06.19
//		+ custom block syntax, thanks to G. van den Hoven
//		+ set_block_syntax()
//		+ tie_loop()
//		+ tie_var()
//		* v1.9
//
//	2003.06.17
//		* parse() works faster, thanks to Sergej Kurakin
//		- remove_nonjs bugfix
//		+ error handler support
//
//	2003.06.16
//		- set_root() bug
//
//	2003.03.14
//		+ process() now accepts parameters as bits, thanks to Audrius Karabanovas
//		+ set_params() set default parameters for process()
//		* v1.8.1
//		
//	2003.03.14
//		+ phpdoc comments
//		* v1.8
//
//	2002.11.13
//		- $block_names no more
//		- bug in extract blocks
//
//	2002.09.24
//		* parse now accpets string instead of handle
//		+ optional() <opt>
//		* root change
//
//	2002.03.23
//		- bug with templates caintaining { a { b }
//		* v1.7.1
//
//	2002.03.03
//		* fopen fread fclose instead of implode(file()), up to 3x faster
//		+ remove_nonjs - remove only variables that have no spaces in them
//		* speed improvements, got rid of list() = each()
//		+ license :]
//		* v1.7
//
//	2002.03.02
//		- deleted space before each line in the parsed template.
//		- error in method error() :]
//		* v1.6.2 note released :]
//
//	2001.12.06
//		- bug then text had only }
//		* v1.6.1
//
//	2001.10.31
//		+ error on unclosed block
//		+ nested blocks
//		* v1.6
//		
//	2001.09.17
//		- fixed bug with 'keep'
//
//	2001.09.02
//		+ get_var_silent()
//
//	2001.08.09
//		+ error handler
//
//	2001.07.04
//		+ one pass substitution
//
//	2001.05.28
//		+ block name recording
//		* v1.5.1
//
//	2001.05.10
//		- bug in documentation
//
//	2001.05.08
//		* first public release v1.5
//
//	2001.04.04
//		* changed blocks setup, constructor parameters change
//		- error bug
//		- some warnings

/**
*/
