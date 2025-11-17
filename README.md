# find-the-difference
class Solution(object):
    def findTheDifference(self, s, t):
        """
        :type s: str
        :type t: str
        :rtype: str
        """
        xor_val = 0

        for ch in s:
            xor_val ^= ord(ch)

        for ch in t:
            xor_val ^= ord(ch)

        return chr(xor_val)
