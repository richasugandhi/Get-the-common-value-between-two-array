# Get-the-common-value-between-two-array in Javascript

<script>

var aa = [1,2,3];
    var bb = [2,3,4,5];
    function intersection(aa,bb){
        aa.sort();bb.sort();
        var i=j=0;ret=[];
        while(i<aa.length && j<bb.length){
                if (aa[i] < bb[j]) {
                    i++;
                }
                else if (bb[j] < aa[i]) {
                    j++;
                }
                else {
                    alert(aa[i]);
                    ret.push(aa[i]);
                    i++, j++;
                }
            }
            return ret;
        }

alert(intersection(aa,bb));

</script>
